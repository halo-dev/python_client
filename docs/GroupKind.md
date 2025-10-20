# GroupKind

GroupKind contains group and kind data only.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**group** | **str** | is group name of Extension. | [optional] 
**kind** | **str** | is kind name of Extension. | [optional] 

## Example

```python
from halo_client.models.group_kind import GroupKind

# TODO update the JSON string below
json = "{}"
# create an instance of GroupKind from a JSON string
group_kind_instance = GroupKind.from_json(json)
# print the JSON string representation of the object
print(GroupKind.to_json())

# convert the object into a dict
group_kind_dict = group_kind_instance.to_dict()
# create an instance of GroupKind from a dict
group_kind_from_dict = GroupKind.from_dict(group_kind_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


