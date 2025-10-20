# ConfigMap

<p>ConfigMap holds configuration data to consume.</p>

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**data** | **Dict[str, str]** |  | [optional] 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 

## Example

```python
from halo_client.models.config_map import ConfigMap

# TODO update the JSON string below
json = "{}"
# create an instance of ConfigMap from a JSON string
config_map_instance = ConfigMap.from_json(json)
# print the JSON string representation of the object
print(ConfigMap.to_json())

# convert the object into a dict
config_map_dict = config_map_instance.to_dict()
# create an instance of ConfigMap from a dict
config_map_from_dict = ConfigMap.from_dict(config_map_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


