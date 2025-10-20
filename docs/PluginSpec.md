# PluginSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**author** | [**PluginAuthor**](PluginAuthor.md) |  | [optional] 
**config_map_name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**homepage** | **str** |  | [optional] 
**issues** | **str** |  | [optional] 
**license** | [**List[License]**](License.md) |  | [optional] 
**logo** | **str** |  | [optional] 
**plugin_dependencies** | **Dict[str, str]** |  | [optional] 
**repo** | **str** |  | [optional] 
**requires** | **str** | SemVer format. | [optional] 
**setting_name** | **str** |  | [optional] 
**version** | **str** | plugin version. | 

## Example

```python
from halo_client.models.plugin_spec import PluginSpec

# TODO update the JSON string below
json = "{}"
# create an instance of PluginSpec from a JSON string
plugin_spec_instance = PluginSpec.from_json(json)
# print the JSON string representation of the object
print(PluginSpec.to_json())

# convert the object into a dict
plugin_spec_dict = plugin_spec_instance.to_dict()
# create an instance of PluginSpec from a dict
plugin_spec_from_dict = PluginSpec.from_dict(plugin_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


