# CommentStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**has_new_reply** | **bool** |  | [optional] 
**last_reply_time** | **datetime** |  | [optional] 
**observed_version** | **int** |  | [optional] 
**reply_count** | **int** |  | [optional] 
**unread_reply_count** | **int** |  | [optional] 
**visible_reply_count** | **int** |  | [optional] 

## Example

```python
from halo_client.models.comment_status import CommentStatus

# TODO update the JSON string below
json = "{}"
# create an instance of CommentStatus from a JSON string
comment_status_instance = CommentStatus.from_json(json)
# print the JSON string representation of the object
print(CommentStatus.to_json())

# convert the object into a dict
comment_status_dict = comment_status_instance.to_dict()
# create an instance of CommentStatus from a dict
comment_status_from_dict = CommentStatus.from_dict(comment_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


