# ChangeOwnPasswordRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**old_password** | **str** | Old password. | 
**password** | **str** | New password. | 

## Example

```python
from halo_client.models.change_own_password_request import ChangeOwnPasswordRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChangeOwnPasswordRequest from a JSON string
change_own_password_request_instance = ChangeOwnPasswordRequest.from_json(json)
# print the JSON string representation of the object
print(ChangeOwnPasswordRequest.to_json())

# convert the object into a dict
change_own_password_request_dict = change_own_password_request_instance.to_dict()
# create an instance of ChangeOwnPasswordRequest from a dict
change_own_password_request_from_dict = ChangeOwnPasswordRequest.from_dict(change_own_password_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


