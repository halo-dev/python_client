# ListedComment

A chunk of items.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**comment** | [**Comment**](Comment.md) |  | 
**owner** | [**OwnerInfo**](OwnerInfo.md) |  | 
**stats** | [**CommentStats**](CommentStats.md) |  | 
**subject** | [**Extension**](Extension.md) |  | [optional] 

## Example

```python
from halo_client.models.listed_comment import ListedComment

# TODO update the JSON string below
json = "{}"
# create an instance of ListedComment from a JSON string
listed_comment_instance = ListedComment.from_json(json)
# print the JSON string representation of the object
print(ListedComment.to_json())

# convert the object into a dict
listed_comment_dict = listed_comment_instance.to_dict()
# create an instance of ListedComment from a dict
listed_comment_from_dict = ListedComment.from_dict(listed_comment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


