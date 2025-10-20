# EmailConfigValidationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** | Gets email display name. | [optional] 
**enable** | **bool** |  | [optional] 
**encryption** | **str** |  | [optional] 
**host** | **str** |  | [optional] 
**password** | **str** |  | [optional] 
**port** | **int** |  | [optional] 
**sender** | **str** | Gets email sender address. | [optional] 
**username** | **str** |  | [optional] 

## Example

```python
from halo_client.models.email_config_validation_request import EmailConfigValidationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EmailConfigValidationRequest from a JSON string
email_config_validation_request_instance = EmailConfigValidationRequest.from_json(json)
# print the JSON string representation of the object
print(EmailConfigValidationRequest.to_json())

# convert the object into a dict
email_config_validation_request_dict = email_config_validation_request_instance.to_dict()
# create an instance of EmailConfigValidationRequest from a dict
email_config_validation_request_from_dict = EmailConfigValidationRequest.from_dict(email_config_validation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


