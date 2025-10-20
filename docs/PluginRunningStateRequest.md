# PluginRunningStateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_async** | **bool** |  | [optional] 
**enable** | **bool** |  | [optional] 

## Example

```python
from halo_client.models.plugin_running_state_request import PluginRunningStateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PluginRunningStateRequest from a JSON string
plugin_running_state_request_instance = PluginRunningStateRequest.from_json(json)
# print the JSON string representation of the object
print(PluginRunningStateRequest.to_json())

# convert the object into a dict
plugin_running_state_request_dict = plugin_running_state_request_instance.to_dict()
# create an instance of PluginRunningStateRequest from a dict
plugin_running_state_request_from_dict = PluginRunningStateRequest.from_dict(plugin_running_state_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


