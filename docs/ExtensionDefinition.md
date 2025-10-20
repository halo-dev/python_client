# ExtensionDefinition

Extension definition.  An {@link ExtensionDefinition ExtensionDefinition} is a type of metadata that provides additional information about  an extension. An extension is a way to add new functionality to an existing class, structure,  enumeration, or protocol type without needing to subclass it.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**ExtensionSpec**](ExtensionSpec.md) |  | 

## Example

```python
from halo_client.models.extension_definition import ExtensionDefinition

# TODO update the JSON string below
json = "{}"
# create an instance of ExtensionDefinition from a JSON string
extension_definition_instance = ExtensionDefinition.from_json(json)
# print the JSON string representation of the object
print(ExtensionDefinition.to_json())

# convert the object into a dict
extension_definition_dict = extension_definition_instance.to_dict()
# create an instance of ExtensionDefinition from a dict
extension_definition_from_dict = ExtensionDefinition.from_dict(extension_definition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


