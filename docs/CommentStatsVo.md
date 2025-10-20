# CommentStatsVo

comment stats value object.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**upvote** | **int** |  | [optional] 

## Example

```python
from halo_client.models.comment_stats_vo import CommentStatsVo

# TODO update the JSON string below
json = "{}"
# create an instance of CommentStatsVo from a JSON string
comment_stats_vo_instance = CommentStatsVo.from_json(json)
# print the JSON string representation of the object
print(CommentStatsVo.to_json())

# convert the object into a dict
comment_stats_vo_dict = comment_stats_vo_instance.to_dict()
# create an instance of CommentStatsVo from a dict
comment_stats_vo_from_dict = CommentStatsVo.from_dict(comment_stats_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


