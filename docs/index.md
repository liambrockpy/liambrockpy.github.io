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

#### GET - Request person with given ID

#### GET - Request house with given ID

#### GET - Request address with given ID

#### GET - Request people within given age range and/or household amount
