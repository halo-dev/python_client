# AuthProvider

Auth provider extension.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**AuthProviderSpec**](AuthProviderSpec.md) |  | 

## Example

```python
from halo_client.models.auth_provider import AuthProvider

# TODO update the JSON string below
json = "{}"
# create an instance of AuthProvider from a JSON string
auth_provider_instance = AuthProvider.from_json(json)
# print the JSON string representation of the object
print(AuthProvider.to_json())

# convert the object into a dict
auth_provider_dict = auth_provider_instance.to_dict()
# create an instance of AuthProvider from a dict
auth_provider_from_dict = AuthProvider.from_dict(auth_provider_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


