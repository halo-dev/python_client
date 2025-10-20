# ReplyVo

A chunk of items.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**Metadata**](Metadata.md) |  | 
**owner** | [**OwnerInfo**](OwnerInfo.md) |  | 
**spec** | [**ReplySpec**](ReplySpec.md) |  | 
**stats** | [**CommentStatsVo**](CommentStatsVo.md) |  | 

## Example

```python
from halo_client.models.reply_vo import ReplyVo

# TODO update the JSON string below
json = "{}"
# create an instance of ReplyVo from a JSON string
reply_vo_instance = ReplyVo.from_json(json)
# print the JSON string representation of the object
print(ReplyVo.to_json())

# convert the object into a dict
reply_vo_dict = reply_vo_instance.to_dict()
# create an instance of ReplyVo from a dict
reply_vo_from_dict = ReplyVo.from_dict(reply_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


