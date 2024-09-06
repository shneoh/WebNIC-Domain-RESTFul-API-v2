# Response Code Reference - Domain API

## Contact 
### Success 2xx 

| Status | Code | Message                        |
| ------ | ---- | ------------------------------ |
| 200    | 1000 | Command completed successfully |

### Endpoints which return data object in "data" field 
* Create Contact 
* Create Contact at Registry 
* Query Contact Info 
* Modify Contact at Registry 
* Modify Contact 

### Endpoints which return other data type in "data" field 
* Replace Contact: Return bulk contact replace task ID 
* Delete Contact: Return contact ID 

### Error 4xx 
| Status | Code/SubCode | Message                                                     |
| ------ | ------------ | ----------------------------------------------------------- |
| 400    | 2400         | System message                                              |
| 400    | DOM2400      | Create contact failed                                       |
| 400    | DOM2400      | Cannot find contact rule                                    |
| 400    | DOM2400      | Cannot find default custom field rule                       |
| 400    | DOM2400      | Contact not found: [contact_id]                             |
| 400    | DOM2400      | [extension] [contact_type] contact country must be MY       |
| 400    | DOM2400      | Error modifying existing contact: [registry_return_message] |
| 400    | DOM2400      | Error creating new contact: [registry_return_message]       |
| 400    | DOM2400      | System failure                                              |
| 400    | DOM2400      | Invalid contact id                                          |
| 400    | DOM2400      | Contact not found                                           |
| 400    | DOM2400      | Contact rule not found                                      |
| 400    | DOM2400      | Invalid domains: [domain_name]                              |
| 400    | DOM2400      | Failed to create bulk task                                  |
| 400    | DOM2400      | Invalid contact: [contact_id]                               |
| 400    | DOM2400      | Contact ID [contact_id] in use                              |
| 400    | DOM4000      | Field Validation Error                                      |
| 400    | DOM5001      | Reseller not found                                          |

### Error 5xx 
| Status | Code/SubCode | Message                |
| ------ | ------------ | ---------------------- |
| 500    | 2400         | System message         |
| 500    | DOM5000      | Unknown error occurred |

 