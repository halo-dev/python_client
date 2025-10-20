# AuthProviderSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**auth_type** | **str** | Auth type: form or oauth2. | 
**authentication_url** | **str** | Authentication url of the auth provider | 
**binding_url** | **str** |  | [optional] 
**config_map_ref** | [**ConfigMapRef**](ConfigMapRef.md) |  | [optional] 
**description** | **str** |  | [optional] 
**display_name** | **str** | Display name of the auth provider | 
**help_page** | **str** |  | [optional] 
**logo** | **str** |  | [optional] 
**method** | **str** |  | [optional] 
**remember_me_support** | **bool** |  | [optional] 
**setting_ref** | [**SettingRef**](SettingRef.md) |  | [optional] 
**unbind_url** | **str** |  | [optional] 
**website** | **str** |  | [optional] 

## Example

```python
from halo_client.models.auth_provider_spec import AuthProviderSpec

# TODO update the JSON string below
json = "{}"
# create an instance of AuthProviderSpec from a JSON string
auth_provider_spec_instance = AuthProviderSpec.from_json(json)
# print the JSON string representation of the object
print(AuthProviderSpec.to_json())

# convert the object into a dict
auth_provider_spec_dict = auth_provider_spec_instance.to_dict()
# create an instance of AuthProviderSpec from a dict
auth_provider_spec_from_dict = AuthProviderSpec.from_dict(auth_provider_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


