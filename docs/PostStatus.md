# PostStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**comments_count** | **int** |  | [optional] 
**conditions** | [**List[Condition]**](Condition.md) |  | [optional] 
**contributors** | **List[str]** |  | [optional] 
**excerpt** | **str** |  | [optional] 
**hide_from_list** | **bool** | see {@link Category.CategorySpec#isHideFromList Category.CategorySpec#isHideFromList()}. | [optional] 
**in_progress** | **bool** |  | [optional] 
**last_modify_time** | **datetime** |  | [optional] 
**observed_version** | **int** |  | [optional] 
**permalink** | **str** |  | [optional] 
**phase** | **str** |  | [optional] 

## Example

```python
from halo_client.models.post_status import PostStatus

# TODO update the JSON string below
json = "{}"
# create an instance of PostStatus from a JSON string
post_status_instance = PostStatus.from_json(json)
# print the JSON string representation of the object
print(PostStatus.to_json())

# convert the object into a dict
post_status_dict = post_status_instance.to_dict()
# create an instance of PostStatus from a dict
post_status_from_dict = PostStatus.from_dict(post_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


