# ReplaceOperation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**op** | **str** |  | 
**path** | **str** | A JSON Pointer path pointing to the location to move/copy from. | 
**value** | **object** | Value can be any JSON value | 

## Example

```python
from halo_client.models.replace_operation import ReplaceOperation

# TODO update the JSON string below
json = "{}"
# create an instance of ReplaceOperation from a JSON string
replace_operation_instance = ReplaceOperation.from_json(json)
# print the JSON string representation of the object
print(ReplaceOperation.to_json())

# convert the object into a dict
replace_operation_dict = replace_operation_instance.to_dict()
# create an instance of ReplaceOperation from a dict
replace_operation_from_dict = ReplaceOperation.from_dict(replace_operation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


