# CopyOperation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_from** | **str** | A JSON Pointer path pointing to the location to move/copy from. | 
**op** | **str** |  | 
**path** | **str** | A JSON Pointer path pointing to the location to move/copy from. | 

## Example

```python
from halo_client.models.copy_operation import CopyOperation

# TODO update the JSON string below
json = "{}"
# create an instance of CopyOperation from a JSON string
copy_operation_instance = CopyOperation.from_json(json)
# print the JSON string representation of the object
print(CopyOperation.to_json())

# convert the object into a dict
copy_operation_dict = copy_operation_instance.to_dict()
# create an instance of CopyOperation from a dict
copy_operation_from_dict = CopyOperation.from_dict(copy_operation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


