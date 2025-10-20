# GroupStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_attachments** | **int** | Total of attachments under the current group | [optional] 
**update_timestamp** | **datetime** | Update timestamp of the group | [optional] 

## Example

```python
from halo_client.models.group_status import GroupStatus

# TODO update the JSON string below
json = "{}"
# create an instance of GroupStatus from a JSON string
group_status_instance = GroupStatus.from_json(json)
# print the JSON string representation of the object
print(GroupStatus.to_json())

# convert the object into a dict
group_status_dict = group_status_instance.to_dict()
# create an instance of GroupStatus from a dict
group_status_from_dict = GroupStatus.from_dict(group_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


