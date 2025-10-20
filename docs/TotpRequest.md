# TotpRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**password** | **str** |  | 
**secret** | **str** |  | 

## Example

```python
from halo_client.models.totp_request import TotpRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TotpRequest from a JSON string
totp_request_instance = TotpRequest.from_json(json)
# print the JSON string representation of the object
print(TotpRequest.to_json())

# convert the object into a dict
totp_request_dict = totp_request_instance.to_dict()
# create an instance of TotpRequest from a dict
totp_request_from_dict = TotpRequest.from_dict(totp_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


