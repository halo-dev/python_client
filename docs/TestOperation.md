# TestOperation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**op** | **str** |  | 
**path** | **str** | A JSON Pointer path pointing to the location to move/copy from. | 
**value** | **object** | Value can be any JSON value | 

## Example

```python
from halo_client.models.test_operation import TestOperation

# TODO update the JSON string below
json = "{}"
# create an instance of TestOperation from a JSON string
test_operation_instance = TestOperation.from_json(json)
# print the JSON string representation of the object
print(TestOperation.to_json())

# convert the object into a dict
test_operation_dict = test_operation_instance.to_dict()
# create an instance of TestOperation from a dict
test_operation_from_dict = TestOperation.from_dict(test_operation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


