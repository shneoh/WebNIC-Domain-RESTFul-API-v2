# Response Code Reference - Domain API

## Domain 
### Success 2xx 

| Status | Code | Message                        |
| ------ | ---- | ------------------------------ |
|200 |1000 |Command completed successfully |
|207 |3000 |[num_of_domain_that_success] of [total_num_of_domain] events processed |

### Endpoints which return data object in "data" field 
1. Check Domain Pattern 
1. Query Domain 
1. Get Domain Info 
1. Get Universal WHOIS Information 
1. Get WebNIC Default Nameservers 
1. Create Host 
1. Modify Host 
1. Get Host Info 
1. Delete Host 
1. Get Host Registered Registries 
1. Register Domain 
1. Renew Domain 
1. Delete Domain 
1. Resend Domain Verification Email 
1. Send Authorization Information 
1. Get Domain Statistics (Without specific statistics type) 
1. Get Top Domain Available List 

### Endpoints which return other data type in "data" field 
1. Count Total Domains: Return the number of domains you own 
2. Upload Verification Document: Return the URL path of the uploaded verification document 
3. Get Domain Statistics (With specific statistics type): Return the total number of the requested statistic type 

### Endpoints which do not return "data" field 
1. Update Domain Status 
1. Update Domain Nameserver 
1. Check Host 
1. Toggle Auto Renew 
1. Toggle Whois Privacy 
1. Toggle Proxy Subscription 
1. Restore Domain 
1. Reset Authorization Information 
1. Modify Registrant Account 
1. Send Login Info 

### Endpoints which return a downloadable file 
1. Download Certificate 
2. Download Verification Document 

### Error 4xx 
| Status | Code/SubCode | Message                                                     |
| ------ | ------------ | ----------------------------------------------------------- |
|400 |2400 |System message 
|400 |DOM0004 |Forbidden access with current ip address 
|400 |DOM2400 |Invalid domain name 
|400 |DOM2400 |Domain extension not supported for [domain_action] 
|400 |DOM2400 |Domain extension not available for [domain_action] 
|400 |DOM2400 |Invalid domain length 
|400 |DOM2400 |[domain_action] failed due to [price_type] not found 
|400 |DOM2400 |[record_type] record not found 
|400 |DOM2400 |Whois server command failure 
|400 |DOM2400 |Domain not found 
|400 |DOM2400 |Invalid domain status. Acceptable values are: [acceptable_domain_status] 
|400 |DOM2400 |Domain does not exist for this reseller 
|400 |DOM2400 |Legacy domain status is invalid 
|400 |DOM2400 |Status modification not allowed for current domain status 
|400 |DOM2400 |Domain extension not supported 
|400 |DOM2400 |Email failed to send 
|400 |DOM2400 |Feature is not supported for this extension 
|400 |DOM2400 |Unable to grab domain info 
|400 |DOM2400 |Object association prohibits operation 
|400 |DOM2400 |All extensions are not supported for query 
|400 |DOM2400 |[action] nameserver error, unable to find extensions for provider: [provider] 
|400 |DOM2400 |Create nameserver error, domain name ‘[domain_name]’ not exists 
|400 |DOM2400 |Duplicate ip 
|400 |DOM2400 |Invalid ip format: [ip] 
|400 |DOM2400 |Invalid nameserver format 
|400 |DOM2400 |Invalid extension 
|400 |DOM2400 |No rule found 
|400 |DOM2400 |IP exceed maximum amount: [max_amount] 
|400 |DOM2400 |IP does not meet minimum amount: [min_amount] 
|400 |DOM2400 |Invalid host 
|400 |DOM2400 |Unknown error 
|400 |DOM2400 |Host [host_name] is not available 
|400 |DOM2400 |No nameserver found 
|400 |DOM2400 |Domain does not belong to you 
|400 |DOM2400 |Cannot find pgid 
|400 |DOM2400 |Query nameserver failed, domain not found 
|400 |DOM2400 |Extension is not supported for query 
|400 |DOM2400 |Nameserver does not exist 
|400 |DOM2400 |Required field missing: 'target' / 'domainList' 
|400 |DOM2400 |Action prohibited for '[domain_status]' status 
|400 |DOM2400 |Failed to subscribe WHOIS Privacy 
|400 |DOM2400 |Whois privacy status for this domain is already [whois_privacy_status] 
|400 |DOM2400 |Domain contact not found 
|400 |DOM2400 |Domain contact handle not found 
|400 |DOM2400 |'action' is required 
|400 |DOM2400 |Domain proxy is not supported for this extension 
|400 |DOM2400 |Unable to [user_action] due to insufficient balance 
|400 |DOM2400 |Domain contact details not found 
|400 |DOM2400 |Refund failure 
|400 |DOM2400 |Invalid action 
|400 |DOM2400 |Invalid terms. Supported terms are [supported_term] 
|400 |DOM2400 |Domain not available 
|400 |DOM2400 |The domain is [domain_type] domain name. Please input ‘[domain_type]’ in domainType parameter 
|400 |DOM2400 |The domain is under re-registration status. Please input 'rereg' in domainType parameter 
|400 |DOM2400 |Registrant does not exist 
|400 |DOM2400 |[contact_type] contact not found 
|400 |DOM2400 |Reseller contact not found 
|400 |DOM2400 |[extension] registrant contact category must be organization if subscribe proxy 
|400 |DOM2400 |Domain proxy is not supported for [reseller_country] partners for [extension] extension 
|400 |DOM2400 |Pending order creation failed 
|400 |DOM2400 |Domain renewal is in progress, please try again later 
|400 |DOM2400 |Please submit a restoration request via classic.webnic.cc 
|400 |DOM2400 |Domain has just been renewed 
|400 |DOM2400 |Domain is renew prohibited 
|400 |DOM2400 |Renewal prohibited (the domain creation date is less than 60days) 
|400 |DOM2400 |Gaining reseller not found 
|400 |DOM2400 |Registrant user not found 
|400 |DOM2400 |Registrant user not under current partner 
|400 |DOM2400 |Domain already registered under current registrar 
|400 |DOM2400 |Transfer request already submitted for the domain 
|400 |DOM2400 |[contact_type] contact id is invalid 
|400 |DOM2400 |Transfer prohibited with current domain status 
|400 |DOM2400 |Please agree domain restoration policy 
|400 |DOM2400 |Domain restoration is not available for current domain extension 
|400 |DOM2400 |renewPeriod not found from graceRule for ext = [extension] 
|400 |DOM2400 |Domain status is not under redemption grace 
|400 |DOM2400 |Your request has been sent to support@webnic.cc and the restoration and renewal fee has been deducted from your account. However, the request still subject to restoration availability. 
|400 |DOM2400 |Invalid reseller 
|400 |DOM2400 |Invalid domain 
|400 |DOM2400 |Domain does not exist 
|400 |DOM2400 |Invalid domain status: [domain_status] 
|400 |DOM2400 |Rule(s) not found 
|400 |DOM2400 |Domain deletion not available 
|400 |DOM2400 |Object status prohibits operation 
|400 |DOM2400 |Invalid certificate language. Acceptable values are: [acceptable_language] 
|400 |DOM2400 |Failed to retrieve auth info. Please reset auth info and try again 
|400 |DOM2400 |Pending order not found 
|400 |DOM2400 |Invalid type, valid type are: [valid_document_type] 
|400 |DOM2400 |Invalid file type. Only [file_type] files are allowed 
|400 |DOM2400 |Please upload a file 
|400 |DOM2400 |File upload failed 
|400 |DOM2400 |No pending verification document record found 
|400 |DOM2400 |Maximum other file upload reached 
|400 |DOM2400 |File type already uploaded: [document_type] 
|400 |DOM2400 |System failure 
|400 |DOM2400 |Record not found 
|400 |DOM2400 |Download failed 
|400 |DOM2400 |Invalid url 
|400 |DOM2400 |Invalid statistics type 
|400 |DOM2400 |Invalid registrant username 
|400 |DOM2400 |Invalid user account 
|400 |DOM2400 |Invalid username 
|400 |DOM4000 |Field Validation Error 
|400 |DOM5001 |Reseller not found 
|400 |DOM5001 |Reseller contact not found 



### Error 5xx 
| Status | Code/SubCode | Message                |
| ------ | ------------ | ---------------------- |
| 500    | 2400         | System message         |
| 500    | DOM5000      | Unknown error occurred |

 