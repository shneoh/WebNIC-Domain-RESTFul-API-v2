# Response Code Reference - Domain API

## Secondhand Domain
### Success 2xx 

| Status | Code | Message                        |
| ------ | ---- | ------------------------------ |
| 200    | 1000 | Command completed successfully |

> This endpoint returns data object in "data" field 

### Error 4xx 
| Status | Code/SubCode | Message                       |
| ------ | ------------ | ----------------------------- |
| 400    | 2400         | System message                |
| 400    | DOM2400      | Reseller not found            |
| 400    | DOM2400      | Record cannot be more than 50 |
| 400    | DOM2400      | Feature are not enable        |






### Error 5xx 
| Status | Code/SubCode | Message                |
| ------ | ------------ | ---------------------- |
| 500    | 2400         | System message         |
| 500    | DOM5000      | Unknown error occurred |

 