# CommentWithReplyVo

A chunk of items.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**Metadata**](Metadata.md) |  | 
**owner** | [**OwnerInfo**](OwnerInfo.md) |  | 
**replies** | [**ListResultReplyVo**](ListResultReplyVo.md) |  | [optional] 
**spec** | [**CommentSpec**](CommentSpec.md) |  | 
**stats** | [**CommentStatsVo**](CommentStatsVo.md) |  | 
**status** | [**CommentStatus**](CommentStatus.md) |  | [optional] 

## Example

```python
from halo_client.models.comment_with_reply_vo import CommentWithReplyVo

# TODO update the JSON string below
json = "{}"
# create an instance of CommentWithReplyVo from a JSON string
comment_with_reply_vo_instance = CommentWithReplyVo.from_json(json)
# print the JSON string representation of the object
print(CommentWithReplyVo.to_json())

# convert the object into a dict
comment_with_reply_vo_dict = comment_with_reply_vo_instance.to_dict()
# create an instance of CommentWithReplyVo from a dict
comment_with_reply_vo_from_dict = CommentWithReplyVo.from_dict(comment_with_reply_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


