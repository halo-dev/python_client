# ExtensionPointSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**class_name** | **str** |  | 
**description** | **str** |  | [optional] 
**display_name** | **str** |  | 
**icon** | **str** |  | [optional] 
**type** | **str** |  | 

## Example

```python
from halo_client.models.extension_point_spec import ExtensionPointSpec

# TODO update the JSON string below
json = "{}"
# create an instance of ExtensionPointSpec from a JSON string
extension_point_spec_instance = ExtensionPointSpec.from_json(json)
# print the JSON string representation of the object
print(ExtensionPointSpec.to_json())

# convert the object into a dict
extension_point_spec_dict = extension_point_spec_instance.to_dict()
# create an instance of ExtensionPointSpec from a dict
extension_point_spec_from_dict = ExtensionPointSpec.from_dict(extension_point_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


