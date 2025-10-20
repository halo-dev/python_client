# FileReverseProxyProvider


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**directory** | **str** |  | [optional] 
**filename** | **str** |  | [optional] 

## Example

```python
from halo_client.models.file_reverse_proxy_provider import FileReverseProxyProvider

# TODO update the JSON string below
json = "{}"
# create an instance of FileReverseProxyProvider from a JSON string
file_reverse_proxy_provider_instance = FileReverseProxyProvider.from_json(json)
# print the JSON string representation of the object
print(FileReverseProxyProvider.to_json())

# convert the object into a dict
file_reverse_proxy_provider_dict = file_reverse_proxy_provider_instance.to_dict()
# create an instance of FileReverseProxyProvider from a dict
file_reverse_proxy_provider_from_dict = FileReverseProxyProvider.from_dict(file_reverse_proxy_provider_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


