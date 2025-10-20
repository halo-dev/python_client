# CommentStats

comment stats value object.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**upvote** | **int** |  | [optional] 

## Example

```python
from halo_client.models.comment_stats import CommentStats

# TODO update the JSON string below
json = "{}"
# create an instance of CommentStats from a JSON string
comment_stats_instance = CommentStats.from_json(json)
# print the JSON string representation of the object
print(CommentStats.to_json())

# convert the object into a dict
comment_stats_dict = comment_stats_instance.to_dict()
# create an instance of CommentStats from a dict
comment_stats_from_dict = CommentStats.from_dict(comment_stats_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


