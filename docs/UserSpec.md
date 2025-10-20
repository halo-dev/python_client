# UserSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**avatar** | **str** |  | [optional] 
**bio** | **str** |  | [optional] 
**disabled** | **bool** |  | [optional] 
**display_name** | **str** |  | 
**email** | **str** |  | 
**email_verified** | **bool** |  | [optional] 
**login_history_limit** | **int** |  | [optional] 
**password** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**registered_at** | **datetime** |  | [optional] 
**totp_encrypted_secret** | **str** |  | [optional] 
**two_factor_auth_enabled** | **bool** |  | [optional] 

## Example

```python
from halo_client.models.user_spec import UserSpec

# TODO update the JSON string below
json = "{}"
# create an instance of UserSpec from a JSON string
user_spec_instance = UserSpec.from_json(json)
# print the JSON string representation of the object
print(UserSpec.to_json())

# convert the object into a dict
user_spec_dict = user_spec_instance.to_dict()
# create an instance of UserSpec from a dict
user_spec_from_dict = UserSpec.from_dict(user_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


