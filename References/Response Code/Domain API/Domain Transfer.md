# Response Code Reference - Domain API

## Domain Transfer
### Success 2xx 

| Status | Code | Message                        |
| ------ | ---- | ------------------------------ |
| 200    | 1000 | Command completed successfully |

### Endpoints which return data object in "data" field 
1. Submit Registrar Transfer In 
2. Get Registrar Transfer In Status by Domain Name 
3. Get Registrar Transfer In Status by Id 
4. Get Registrar Transfer Away Status by Domain Name 
5. Get Registrar Transfer Away Status by Id 
6. Submit Reseller Transfer 
7. Get Reseller Transfer Status by Domain Name 
8. Get Reseller Transfer Status by Id 

### Endpoints which do not return "data" field 
1. Update Registrar Transfer Away Status 
2. Update Reseller Transfer Away Status 

### Error 4xx 
| Status | Code/SubCode | Message                                                                                                                                              |
| ------ | ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| 400    | 2400         | System message                                                                                                                                       |
| 400    | DOM2400      | Invalid domain name                                                                                                                                  |
| 400    | DOM2400      | [reseller_type] not found                                                                                                                            |
| 400    | DOM2400      | Registrant user not found                                                                                                                            |
| 400    | DOM2400      | Registrant user not under current partner                                                                                                            |
| 400    | DOM2400      | Domain already registered under current registrar                                                                                                    |
| 400    | DOM2400      | Transfer request already submitted for the domain                                                                                                    |
| 400    | DOM2400      | [contact_id] contact id is invalid                                                                                                                   |
| 400    | DOM2400      | [contact_type] contact not found                                                                                                                     |
| 400    | DOM2400      | Domain extension not supported                                                                                                                       |
| 400    | DOM2400      | Domain extension not supported for query                                                                                                             |
| 400    | DOM2400      | Domain extension not available for query                                                                                                             |
| 400    | DOM2400      | Invalid domain length                                                                                                                                |
| 400    | DOM2400      | [domain_action] failed due to price not found                                                                                                        |
| 400    | DOM2400      | The domain is premium name. Please input 'premium' in domainType parameter                                                                           |
| 400    | DOM2400      | Proxy is not supported for this extension                                                                                                            |
| 400    | DOM2400      | Contact proxy information were detected as being manually input, please subscribe to our proxy service if you wish to take advantage of that feature |
| 400    | DOM2400      | Domain transfer price not found                                                                                                                      |
| 400    | DOM2400      | Domain transfer proxy price not found                                                                                                                |
| 400    | DOM2400      | Insufficient balance for domain transfer                                                                                                             |
| 400    | DOM2400      | Transfer prohibited with current domain status                                                                                                       |
| 400    | DOM2400      | Pending order creation failed                                                                                                                        |
| 400    | DOM2400      | Reseller contact not found                                                                                                                           |
| 400    | DOM2400      | Requestor contact not found                                                                                                                          |
| 400    | DOM2400      | Transfer in record not found                                                                                                                         |
| 400    | DOM2400      | Domain under transfer status by other reseller                                                                                                       |
| 400    | DOM2400      | Domain transfer away record not found                                                                                                                |
| 400    | DOM2400      | Record not found                                                                                                                                     |
| 400    | DOM2400      | Invalid domain transfer away approve type                                                                                                            |
| 400    | DOM2400      | Invalid approval credentials                                                                                                                         |
| 400    | DOM2400      | [reseller_type] contact not found                                                                                                                    |
| 400    | DOM2400      | Domain already under current partner                                                                                                                 |
| 400    | DOM2400      | Domain not found                                                                                                                                     |
| 400    | DOM2400      | Domain is under transferring away process                                                                                                            |
| 400    | DOM2400      | [reseller_type] contact email not found                                                                                                              |
| 400    | DOM2400      | Unable to submit transfer due to insufficient balance                                                                                                |
| 400    | DOM2400      | Transfer record not found                                                                                                                            |
| 400    | DOM2400      | Transfer not yet approved                                                                                                                            |
| 400    | DOM2400      | Current domain contacts not found                                                                                                                    |
| 400    | DOM2400      | Losing reseller domain [contact_type] contact not found                                                                                              |
| 400    | DOM2400      | Create contact failed                                                                                                                                |
| 400    | DOM2400      | Cannot find contact rule                                                                                                                             |
| 400    | DOM2400      | Cannot find default custom field rule                                                                                                                |
| 400    | DOM2400      | Contact not found: [contact_id]                                                                                                                      |
| 400    | DOM2400      | [extension] [contact_type] contact country must be MY                                                                                                |
| 400    | DOM2400      | Error modifying existing contact: [registry_return_message]                                                                                          |
| 400    | DOM2400      | Error creating new contact: [registry_return_message]                                                                                                |
| 400    | DOM2400      | System failure                                                                                                                                       |
| 400    | DOM2400      | Unable to renew domain due to payment failure                                                                                                        |
| 400    | DOM2400      | Invalid domain reseller transfer approve type                                                                                                        |
| 400    | DOM4000      | Field Validation Error                                                                                                                               |
| 400    | DOM5001      | Reseller not found                                                                                                                                   |





### Error 5xx 
| Status | Code/SubCode | Message                |
| ------ | ------------ | ---------------------- |
| 500    | 2400         | System message         |
| 500    | DOM5000      | Unknown error occurred |

 