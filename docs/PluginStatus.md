# PluginStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conditions** | [**List[Condition]**](Condition.md) |  | [optional] 
**entry** | **str** |  | [optional] 
**last_probe_state** | **str** |  | [optional] 
**last_start_time** | **datetime** |  | [optional] 
**load_location** | **str** | Load location of the plugin, often a path. | [optional] 
**logo** | **str** |  | [optional] 
**phase** | **str** |  | [optional] 
**stylesheet** | **str** |  | [optional] 

## Example

```python
from halo_client.models.plugin_status import PluginStatus

# TODO update the JSON string below
json = "{}"
# create an instance of PluginStatus from a JSON string
plugin_status_instance = PluginStatus.from_json(json)
# print the JSON string representation of the object
print(PluginStatus.to_json())

# convert the object into a dict
plugin_status_dict = plugin_status_instance.to_dict()
# create an instance of PluginStatus from a dict
plugin_status_from_dict = PluginStatus.from_dict(plugin_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


