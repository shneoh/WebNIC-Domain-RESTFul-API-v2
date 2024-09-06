# Response Code Reference - Domain API

## Domain Broker 
### Success 2xx 

| Status | Code | Message                        |
| ------ | ---- | ------------------------------ |
| 200    | 1000 | Command completed successfully |

> This endpoint does not return "data" field
### Error 4xx 
| Status | Code/SubCode | Message                                                 |
| ------ | ------------ | ------------------------------------------------------- |
| 400    | 2400         | System message                                          |
| 400    | DOM2400      | Reseller not found                                      |
| 400    | DOM2400      | Minimum amount is 1.00                                  |
| 400    | DOM2400      | Invalid domain name                                     |
| 400    | DOM2400      | Domain not under WebNIC                                 |
| 400    | DOM2400      | Unable to establish broker service on self-owned domain |
| 400    | DOM2400      | Email failed to send                                    |


### Error 5xx 
| Status | Code/SubCode | Message                |
| ------ | ------------ | ---------------------- |
| 500    | 2400         | System message         |
| 500    | DOM5000      | Unknown error occurred |

 