# ReasonTypeInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**ui_permissions** | **List[str]** |  | [optional] 

## Example

```python
from halo_client.models.reason_type_info import ReasonTypeInfo

# TODO update the JSON string below
json = "{}"
# create an instance of ReasonTypeInfo from a JSON string
reason_type_info_instance = ReasonTypeInfo.from_json(json)
# print the JSON string representation of the object
print(ReasonTypeInfo.to_json())

# convert the object into a dict
reason_type_info_dict = reason_type_info_instance.to_dict()
# create an instance of ReasonTypeInfo from a dict
reason_type_info_from_dict = ReasonTypeInfo.from_dict(reason_type_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


