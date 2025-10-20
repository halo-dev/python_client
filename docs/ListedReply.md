# ListedReply

A chunk of items.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**owner** | [**OwnerInfo**](OwnerInfo.md) |  | 
**reply** | [**Reply**](Reply.md) |  | 
**stats** | [**CommentStats**](CommentStats.md) |  | 

## Example

```python
from halo_client.models.listed_reply import ListedReply

# TODO update the JSON string below
json = "{}"
# create an instance of ListedReply from a JSON string
listed_reply_instance = ListedReply.from_json(json)
# print the JSON string representation of the object
print(ListedReply.to_json())

# convert the object into a dict
listed_reply_dict = listed_reply_instance.to_dict()
# create an instance of ListedReply from a dict
listed_reply_from_dict = ListedReply.from_dict(listed_reply_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


