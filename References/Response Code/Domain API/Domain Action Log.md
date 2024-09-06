# Response Code Reference - Domain API

## Domain Action Log 
### Success 2xx 

| Status | Code | Message                        |
| ------ | ---- | ------------------------------ |
| 200    | 1000 | Command completed successfully |

> This endpoint returns data object in "data" field

### Error 4xx 
| Status | Code/SubCode | Message                 |
| ------ | ------------ | ----------------------- |
| 400    | 2400         | System message          |
| 400    | DOM2400      | Domain log not found    |
| 400    | DOM2400      | Domain record not found |
| 400    | DOM5001      | Reseller not found      |



### Error 5xx 
| Status | Code/SubCode | Message                |
| ------ | ------------ | ---------------------- |
| 500    | 2400         | System message         |
| 500    | DOM5000      | Unknown error occurred |

 