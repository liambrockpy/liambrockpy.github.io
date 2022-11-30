# PUT

## PUT - Update existing or add new person to database

`api/people/:id/update?name=name&age=number&householdAmount=number`

### Parameter

| Field      | Type |
| ----------- | ----------- |
| Name      | String       |
| Age   | Int        |
| Household Amount   | Int        |

### Error 400
| Name      | Description |
| ----------- | ----------- |
| Person      | Person was not updated       |



### Error 400
| Name      | Description |
| ----------- | ----------- |
| Person      | Person was not updated       |

res: 200/201/400, body: new/updated/error data

## PUT - Update existing or add new house to database

`api/houses/:id/update?peopleId=id&addressId=id`

### Parameter

| Field      | Type |
| ----------- | ----------- |
| People Id      | Int       |
| Address Id   | Int        |



res: 200/201/400, body: new/updated/error data

## PUT - Update existing or add new address to database

`api/addresses/:id/update?postcode=code&street=name`

### Parameter

| Field      | Type |
| ----------- | ----------- |
| Postcode     | String       |
| Street  | String        |


res: 200/201, body: new/updated/error data
