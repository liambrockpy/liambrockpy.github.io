# Neighbourhood API

### An API service that serves information about people and their houses

---

## GET

#### GET - Request all people / houses / addresses

`/api/people`
`/api/houses`
`/api/addresses`

#### Success 200

##### People

| Field           | Type   |
| --------------- | ------ |
| id              | int    |
| name            | String |
| age             | int    |
| householdAmount | int    |

##### Houses

| Field     | Type |
| --------- | ---- |
| id        | int  |
| addressId | int  |
| ownerId   | int  |

##### Addresses

| Field    | Type   |
| -------- | ------ |
| id       | int    |
| postcode | String |
| street   | String |

#### GET - Request person / house / address with given ID

`/api/people/:id`
`/api/houses/:id`
`/api/addresses/:id`

#### GET - Request people within given age range and/or household amount

`/api/people?minAge=0&maxAge=130`
| Field | Type | Description
| ----- | ---- | -------
| minAge | int | Minimum age value<br />Range minimum value: `0`
| maxAge | int | Maximum age value<br />Range maximum value: `130`
`/api/people?householdAmount=4`
| Field | Type | Description
| --------------- | ---- | -------
| householdAmount | int | Minimum age value<br />Range: `0` - `20`
`/api/people?minAge={int}&maxAge={int}&householdAmount={int}`
