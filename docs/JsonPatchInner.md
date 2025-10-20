# JsonPatchInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**op** | **str** |  | 
**path** | **str** | A JSON Pointer path pointing to the location to move/copy from. | 
**value** | **object** | Value can be any JSON value | 
**var_from** | **str** | A JSON Pointer path pointing to the location to move/copy from. | 

## Example

```python
from halo_client.models.json_patch_inner import JsonPatchInner

# TODO update the JSON string below
json = "{}"
# create an instance of JsonPatchInner from a JSON string
json_patch_inner_instance = JsonPatchInner.from_json(json)
# print the JSON string representation of the object
print(JsonPatchInner.to_json())

# convert the object into a dict
json_patch_inner_dict = json_patch_inner_instance.to_dict()
# create an instance of JsonPatchInner from a dict
json_patch_inner_from_dict = JsonPatchInner.from_dict(json_patch_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


