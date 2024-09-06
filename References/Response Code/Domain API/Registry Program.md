# Response Code Reference - Domain API

## Registry Program
### Success 2xx 

| Status | Code | Message                        |
| ------ | ---- | ------------------------------ |
| 200    | 1000 | Command completed successfully |

### Endpoints which return other data type in "data" field 
1. Check Free TW Domain Eligibility: Return the TW domain eligibility 

### Endpoints which do not return "data" field 
1. Bundle HK Domain 
2. SGNIC Reserve Domain 
3. SGNIC Activate Domain  

### Error 4xx 
| Status | Code/SubCode | Message                                                                                                                                   |
| ------ | ------------ | ----------------------------------------------------------------------------------------------------------------------------------------- |
| 400    | 2400         | System message                                                                                                                            |
| 400    | DOM2400      | Invalid domain name                                                                                                                       |
| 400    | DOM2400      | This bundle program is for .hk domain only                                                                                                |
| 400    | DOM2400      | Domain name, [domain_name] is not found                                                                                                   |
| 400    | DOM2400      | Bundle domain name must be an IDN domain                                                                                                  |
| 400    | DOM2400      | Domain name, [domain_name] is not inserted                                                                                                |
| 400    | DOM2400      | Domain contact is not found                                                                                                               |
| 400    | DOM2400      | Domain contact details, [contact_id] not found                                                                                            |
| 400    | DOM2400      | Domain name exists                                                                                                                        |
| 400    | DOM2400      | Your application was failed due to the verification has validated over 24 hours. Please contact support@webnic.cc for further assistance. |
| 400    | DOM2400      | Internal Server Error. Please contact support                                                                                             |
| 400    | DOM2400      | Basic Input Check (for example, query format, length of UBN, or no value)                                                                 |
| 400    | DOM2400      | Wrong Domain Type (for example, org.tw or net.tw)                                                                                         |
| 400    | DOM2400      | The UBN has been used in this program                                                                                                     |
| 400    | DOM2400      | The UBN is not in the MOEA's categories of 'Company', 'Branch Office' or 'Business'                                                     |
| 400    | DOM2400      | Chinese Company Name is not matched                                                                                                       |
| 400    | DOM2400      | Company Registration is over 1 year                                                                                                       |
| 400    | DOM2400      | TWNIC DB Connection Error                                                                                                                 |
| 400    | DOM2400      | MOEA GCIS Connection Error                                                                                                                |
| 400    | DOM2400      | MOEA GCIS System Busy                                                                                                                     |
| 400    | DOM2400      | MOEA GCIS Format Unidentified                                                                                                             |
| 400    | DOM2400      | MOEA GCIST Too Many Data Returned                                                                                                         |
| 400    | DOM2400      | Create contact failed: Create contact failed                                                                                              |
| 400    | DOM2400      | Create contact at registry failed: [validation_error_response]: [create_contact_at_registry_error_response]                               |
| 400    | DOM2400      | Post reservation failed: [registry_return_message]                                                                                        |
| 400    | DOM2400      | Unable to activate domain name due to insufficient balance                                                                                |
| 400    | DOM2400      | No corresponding reservation found                                                                                                        |
| 400    | DOM2400      | Failed to insert record into system                                                                                                       |
| 400    | DOM2400      | Create contact failed                                                                                                                     |
| 400    | DOM2400      | Domain name not in reservePeriod                                                                                                          |
| 400    | DOM2400      | Domain name does not exist                                                                                                                |
| 400    | DOM4000      | Field Validation Error                                                                                                                    |
| 400    | DOM5001      | Reseller not found                                                                                                                        |






### Error 5xx 
| Status | Code/SubCode | Message                |
| ------ | ------------ | ---------------------- |
| 500    | 2400         | System message         |
| 500    | DOM5000      | Unknown error occurred |

 