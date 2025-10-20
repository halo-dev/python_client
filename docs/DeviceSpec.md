# DeviceSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ip_address** | **str** |  | 
**last_accessed_time** | **datetime** |  | [optional] 
**last_authenticated_time** | **datetime** |  | [optional] 
**principal_name** | **str** |  | 
**remember_me_series_id** | **str** |  | [optional] 
**session_id** | **str** |  | 
**user_agent** | **str** |  | [optional] 

## Example

```python
from halo_client.models.device_spec import DeviceSpec

# TODO update the JSON string below
json = "{}"
# create an instance of DeviceSpec from a JSON string
device_spec_instance = DeviceSpec.from_json(json)
# print the JSON string representation of the object
print(DeviceSpec.to_json())

# convert the object into a dict
device_spec_dict = device_spec_instance.to_dict()
# create an instance of DeviceSpec from a dict
device_spec_from_dict = DeviceSpec.from_dict(device_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


