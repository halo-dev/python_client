# ExtensionSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**class_name** | **str** |  | 
**description** | **str** |  | [optional] 
**display_name** | **str** |  | 
**extension_point_name** | **str** |  | 
**icon** | **str** |  | [optional] 

## Example

```python
from halo_client.models.extension_spec import ExtensionSpec

# TODO update the JSON string below
json = "{}"
# create an instance of ExtensionSpec from a JSON string
extension_spec_instance = ExtensionSpec.from_json(json)
# print the JSON string representation of the object
print(ExtensionSpec.to_json())

# convert the object into a dict
extension_spec_dict = extension_spec_instance.to_dict()
# create an instance of ExtensionSpec from a dict
extension_spec_from_dict = ExtensionSpec.from_dict(extension_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


