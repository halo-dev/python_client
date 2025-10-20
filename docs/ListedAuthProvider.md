# ListedAuthProvider

A listed value object for {@link run.halo.app.core.extension.AuthProvider run.halo.app.core.extension.AuthProvider}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**auth_type** | **str** |  | [optional] 
**authentication_url** | **str** |  | [optional] 
**binding_url** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**display_name** | **str** |  | 
**enabled** | **bool** |  | [optional] 
**help_page** | **str** |  | [optional] 
**is_bound** | **bool** |  | [optional] 
**logo** | **str** |  | [optional] 
**name** | **str** |  | 
**priority** | **int** |  | [optional] 
**privileged** | **bool** |  | [optional] 
**supports_binding** | **bool** |  | [optional] 
**unbinding_url** | **str** |  | [optional] 
**website** | **str** |  | [optional] 

## Example

```python
from halo_client.models.listed_auth_provider import ListedAuthProvider

# TODO update the JSON string below
json = "{}"
# create an instance of ListedAuthProvider from a JSON string
listed_auth_provider_instance = ListedAuthProvider.from_json(json)
# print the JSON string representation of the object
print(ListedAuthProvider.to_json())

# convert the object into a dict
listed_auth_provider_dict = listed_auth_provider_instance.to_dict()
# create an instance of ListedAuthProvider from a dict
listed_auth_provider_from_dict = ListedAuthProvider.from_dict(listed_auth_provider_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


