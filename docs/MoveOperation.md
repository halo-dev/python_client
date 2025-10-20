# MoveOperation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_from** | **str** | A JSON Pointer path pointing to the location to move/copy from. | 
**op** | **str** |  | 
**path** | **str** | A JSON Pointer path pointing to the location to move/copy from. | 

## Example

```python
from halo_client.models.move_operation import MoveOperation

# TODO update the JSON string below
json = "{}"
# create an instance of MoveOperation from a JSON string
move_operation_instance = MoveOperation.from_json(json)
# print the JSON string representation of the object
print(MoveOperation.to_json())

# convert the object into a dict
move_operation_dict = move_operation_instance.to_dict()
# create an instance of MoveOperation from a dict
move_operation_from_dict = MoveOperation.from_dict(move_operation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


