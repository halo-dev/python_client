# PluginAuthor


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**website** | **str** |  | [optional] 

## Example

```python
from halo_client.models.plugin_author import PluginAuthor

# TODO update the JSON string below
json = "{}"
# create an instance of PluginAuthor from a JSON string
plugin_author_instance = PluginAuthor.from_json(json)
# print the JSON string representation of the object
print(PluginAuthor.to_json())

# convert the object into a dict
plugin_author_dict = plugin_author_instance.to_dict()
# create an instance of PluginAuthor from a dict
plugin_author_from_dict = PluginAuthor.from_dict(plugin_author_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


