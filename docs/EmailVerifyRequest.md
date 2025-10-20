# EmailVerifyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 

## Example

```python
from halo_client.models.email_verify_request import EmailVerifyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EmailVerifyRequest from a JSON string
email_verify_request_instance = EmailVerifyRequest.from_json(json)
# print the JSON string representation of the object
print(EmailVerifyRequest.to_json())

# convert the object into a dict
email_verify_request_dict = email_verify_request_instance.to_dict()
# create an instance of EmailVerifyRequest from a dict
email_verify_request_from_dict = EmailVerifyRequest.from_dict(email_verify_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


