# API Response Message Reference
## Example Success Response
```JSON
{
  "code": "return_code", 
  "message": "return_message", 
  "data": {return_data_object}
}
```

### Success Response Parameters
| Name      |  Type  | Description        |
| :-------- | :----: | :----------------- |
| `code`    | String | Return code        |
| `message` | String | Return message     |
| `data`    | Object | Return data object |

## Example Error Response
```JSON
{ 
  "code": "return_code", 
  "message": "return_message", 
  "error": { 
      "subCode": "sub_error_code", 
      "message": "sub_error_message" 
  }, 
  "fieldErrors": { 
      "field": "field_name", 
      "message": ["validation_error_message_1", ...] 
  }, 
  "validationErrors": { 
      "field": "field_name", 
      "message": "validation_error_message" 
  } 
} 
```

### Error Response Parameters
| Name                          |   Type   | Description                         |
| :---------------------------- | :------: | :---------------------------------- |
| `code`                        |  String  | Return code                         |
| `message`                     |  String  | Return message                      |
| `error`                       |  Object  | Error object                        |
| ...`subcode`                  |  String  | Sub error code                      |
| ...`message`                  |  String  | Sub error message                   |
| `fieldErrors` (optional)      | Object[] | Request body field validation error |
| ...`field`                    |  String  | Field name                          |
| ...`messages`                 | String[] | Validation error message list       |
| `validationErrors` (optional) | Object[] | Request body validation error       |
| ...`field`                    |  String  | Field name                          |
| ...`message`                  |  String  | Validation error message            |

