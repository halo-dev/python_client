# CommentVo

A chunk of items.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**Metadata**](Metadata.md) |  | 
**owner** | [**OwnerInfo**](OwnerInfo.md) |  | 
**spec** | [**CommentSpec**](CommentSpec.md) |  | 
**stats** | [**CommentStatsVo**](CommentStatsVo.md) |  | 
**status** | [**CommentStatus**](CommentStatus.md) |  | [optional] 

## Example

```python
from halo_client.models.comment_vo import CommentVo

# TODO update the JSON string below
json = "{}"
# create an instance of CommentVo from a JSON string
comment_vo_instance = CommentVo.from_json(json)
# print the JSON string representation of the object
print(CommentVo.to_json())

# convert the object into a dict
comment_vo_dict = comment_vo_instance.to_dict()
# create an instance of CommentVo from a dict
comment_vo_from_dict = CommentVo.from_dict(comment_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


