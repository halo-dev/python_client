# ReverseProxyRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file** | [**FileReverseProxyProvider**](FileReverseProxyProvider.md) |  | [optional] 
**path** | **str** |  | [optional] 

## Example

```python
from halo_client.models.reverse_proxy_rule import ReverseProxyRule

# TODO update the JSON string below
json = "{}"
# create an instance of ReverseProxyRule from a JSON string
reverse_proxy_rule_instance = ReverseProxyRule.from_json(json)
# print the JSON string representation of the object
print(ReverseProxyRule.to_json())

# convert the object into a dict
reverse_proxy_rule_dict = reverse_proxy_rule_instance.to_dict()
# create an instance of ReverseProxyRule from a dict
reverse_proxy_rule_from_dict = ReverseProxyRule.from_dict(reverse_proxy_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


