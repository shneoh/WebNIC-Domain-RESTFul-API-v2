# Response Code Reference - Domain API

## Registrant
### Success 2xx 

| Status | Code | Message                        |
| ------ | ---- | ------------------------------ |
| 200    | 1000 | Command completed successfully |

### Endpoints which return data object in "data" field 
1. Create Registrant Account 
1. Get Registrant Account List 

### Error 4xx 
| Status | Code/SubCode | Message                                                 |
| ------ | ------------ | ------------------------------------------------------- |
| 400    | 2400         | System message                                          |
| 400    | DOM2400      | Invalid username input                                  |
| 400    | DOM2400      | The minimum length of the username is [username_length] |
| 400    | DOM2400      | Registrant account username not available               |
| 400    | DOM5001      | Reseller not found                                      |





### Error 5xx 
| Status | Code/SubCode | Message                |
| ------ | ------------ | ---------------------- |
| 500    | 2400         | System message         |
| 500    | DOM5000      | Unknown error occurred |

 