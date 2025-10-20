# ReverseProxyList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**first** | **bool** | Indicates whether current page is the first page. | 
**has_next** | **bool** | Indicates whether current page has previous page. | 
**has_previous** | **bool** | Indicates whether current page has previous page. | 
**items** | [**List[ReverseProxy]**](ReverseProxy.md) | A chunk of items. | 
**last** | **bool** | Indicates whether current page is the last page. | 
**page** | **int** | Page number, starts from 1. If not set or equal to 0, it means no pagination. | 
**size** | **int** | Size of each page. If not set or equal to 0, it means no pagination. | 
**total** | **int** | Total elements. | 
**total_pages** | **int** | Indicates total pages. | 

## Example

```python
from halo_client.models.reverse_proxy_list import ReverseProxyList

# TODO update the JSON string below
json = "{}"
# create an instance of ReverseProxyList from a JSON string
reverse_proxy_list_instance = ReverseProxyList.from_json(json)
# print the JSON string representation of the object
print(ReverseProxyList.to_json())

# convert the object into a dict
reverse_proxy_list_dict = reverse_proxy_list_instance.to_dict()
# create an instance of ReverseProxyList from a dict
reverse_proxy_list_from_dict = ReverseProxyList.from_dict(reverse_proxy_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


