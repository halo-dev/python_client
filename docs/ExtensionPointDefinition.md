# ExtensionPointDefinition

Extension point definition.  An {@link ExtensionPointDefinition ExtensionPointDefinition} is a concept used in <code>Halo</code> to allow for the  dynamic extension of system. It defines a location within <code>Halo</code> where  additional functionality can be added through the use of plugins or extensions.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**ExtensionPointSpec**](ExtensionPointSpec.md) |  | 

## Example

```python
from halo_client.models.extension_point_definition import ExtensionPointDefinition

# TODO update the JSON string below
json = "{}"
# create an instance of ExtensionPointDefinition from a JSON string
extension_point_definition_instance = ExtensionPointDefinition.from_json(json)
# print the JSON string representation of the object
print(ExtensionPointDefinition.to_json())

# convert the object into a dict
extension_point_definition_dict = extension_point_definition_instance.to_dict()
# create an instance of ExtensionPointDefinition from a dict
extension_point_definition_from_dict = ExtensionPointDefinition.from_dict(extension_point_definition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


