# Patch

## Patch - Update existing person by id

`api/people/:id/update?name=name&age=number&householdAmount=number`

### Parameter

| Field      | Type |
| ----------- | ----------- |
| Name      | String       |
| Age   | Int        |
| Household Amount   | Int        |

### Error 404
| Name      | Description |
| ----------- | ----------- |
| Person      | No person found for specified ID       |

### Error 400
| Name      | Description |
| ----------- | ----------- |
| Person      | Person was not updated       |


res: 200/404/400, 
body: updated/error data

## Patch - Update existing house by id

`api/houses/:id/update?peopleId=id&addressId=id`

### Parameter

| Field      | Type |
| ----------- | ----------- |
| People Id      | Int       |
| Address Id   | Int        |

### Error 404
| Name      | Description |
| ----------- | ----------- |
| House      | No house found for specified ID       |

### Error 400
| Name      | Description |
| ----------- | ----------- |
| House      | House was not updated       |

res: 200/404/400, 
body: updated/error data

## Patch - Update existing address by id

`api/addresses/:id/update?postcode=code&street=name`

### Parameter

| Field      | Type |
| ----------- | ----------- |
| Postcode     | String       |
| Street  | String        |


### Error 404
| Name      | Description |
| ----------- | ----------- |
| Address      | No address found for specified ID       |

### Error 400
| Name      | Description |
| ----------- | ----------- |
| Address      | Address was not updated       |

res: 200/404/400, 
body: updated/error data
