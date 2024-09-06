# Response Code Reference - Domain API

## Domain DNSSEC 
### Success 2xx 

| Status | Code | Message                        |
| ------ | ---- | ------------------------------ |
| 200    | 1000 | Command completed successfully |

### Endpoints which return data object in "data" field 
1. Check DNSSEC Supported 
2. Get DNSSEC Info 

### Endpoints which do not return "data" field 
1. Update DNSSEC 
2. Delete DNSSEC 

### Error 4xx 
| Status | Code/SubCode | Message                                 |
| ------ | ------------ | --------------------------------------- |
| 400    | 2400         | System message                          |
| 400    | DOM2400      | Dnssec not supported for current domain |
| 400    | DOM2400      | No dnssec data to update                |
| 400    | DOM4000      | Field Validation Error                  |
| 400    | DOM5001      | Reseller not found                      |



### Error 5xx 
| Status | Code/SubCode | Message                                                                       |
| ------ | ------------ | ----------------------------------------------------------------------------- |
| 500    | 2400         | System message                                                                |
| 500    | DOM5000      | Check is domain support for dnssec failed                                     |
| 500    | DOM5000      | Unknown error occurred                                                        |
| 500    | DOM5000      | Get domain dnssec info failed                                                 |
| 500    | DOM5000      | Object does not exist                                                         |
| 500    | DOM5000      | Update domain dnssec failed                                                   |
| 500    | DOM5000      | Parameter value policy error \| Digest for type SHA-384 should have length 96 |
| 500    | DOM5000      | Remove domain dnssec failed                                                   |



 