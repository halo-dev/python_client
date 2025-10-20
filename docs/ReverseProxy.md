# ReverseProxy

<p>The reverse proxy custom resource is used to configure a path to proxy it to a directory or  file.</p>  <p>HTTP proxy may be added in the future.</p>

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**rules** | [**List[ReverseProxyRule]**](ReverseProxyRule.md) |  | [optional] 

## Example

```python
from halo_client.models.reverse_proxy import ReverseProxy

# TODO update the JSON string below
json = "{}"
# create an instance of ReverseProxy from a JSON string
reverse_proxy_instance = ReverseProxy.from_json(json)
# print the JSON string representation of the object
print(ReverseProxy.to_json())

# convert the object into a dict
reverse_proxy_dict = reverse_proxy_instance.to_dict()
# create an instance of ReverseProxy from a dict
reverse_proxy_from_dict = ReverseProxy.from_dict(reverse_proxy_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


