# ReasonTypeNotifierMatrix


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**notifiers** | [**List[NotifierInfo]**](NotifierInfo.md) |  | [optional] 
**reason_types** | [**List[ReasonTypeInfo]**](ReasonTypeInfo.md) |  | [optional] 
**state_matrix** | **List[List[bool]]** |  | [optional] 

## Example

```python
from halo_client.models.reason_type_notifier_matrix import ReasonTypeNotifierMatrix

# TODO update the JSON string below
json = "{}"
# create an instance of ReasonTypeNotifierMatrix from a JSON string
reason_type_notifier_matrix_instance = ReasonTypeNotifierMatrix.from_json(json)
# print the JSON string representation of the object
print(ReasonTypeNotifierMatrix.to_json())

# convert the object into a dict
reason_type_notifier_matrix_dict = reason_type_notifier_matrix_instance.to_dict()
# create an instance of ReasonTypeNotifierMatrix from a dict
reason_type_notifier_matrix_from_dict = ReasonTypeNotifierMatrix.from_dict(reason_type_notifier_matrix_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


