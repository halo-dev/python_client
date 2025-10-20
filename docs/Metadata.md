# Metadata

Metadata of Extension.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**annotations** | **Dict[str, str]** | Annotations are like key-value format. | [optional] 
**creation_timestamp** | **datetime** | Creation timestamp of the Extension. | [optional] 
**deletion_timestamp** | **datetime** | Deletion timestamp of the Extension. | [optional] 
**finalizers** | **List[Optional[str]]** |  | [optional] 
**generate_name** | **str** | The name field will be generated automatically according to the given generateName field | [optional] 
**labels** | **Dict[str, str]** | Labels are like key-value format. | [optional] 
**name** | **str** | Metadata name | 
**version** | **int** | Current version of the Extension. It will be bumped up every update. | [optional] 

## Example

```python
from halo_client.models.metadata import Metadata

# TODO update the JSON string below
json = "{}"
# create an instance of Metadata from a JSON string
metadata_instance = Metadata.from_json(json)
# print the JSON string representation of the object
print(Metadata.to_json())

# convert the object into a dict
metadata_dict = metadata_instance.to_dict()
# create an instance of Metadata from a dict
metadata_from_dict = Metadata.from_dict(metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


