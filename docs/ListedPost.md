# ListedPost

A chunk of items.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**categories** | [**List[Category]**](Category.md) |  | 
**contributors** | [**List[Contributor]**](Contributor.md) |  | 
**owner** | [**Contributor**](Contributor.md) |  | 
**post** | [**Post**](Post.md) |  | 
**stats** | [**Stats**](Stats.md) |  | 
**tags** | [**List[Tag]**](Tag.md) |  | 

## Example

```python
from halo_client.models.listed_post import ListedPost

# TODO update the JSON string below
json = "{}"
# create an instance of ListedPost from a JSON string
listed_post_instance = ListedPost.from_json(json)
# print the JSON string representation of the object
print(ListedPost.to_json())

# convert the object into a dict
listed_post_dict = listed_post_instance.to_dict()
# create an instance of ListedPost from a dict
listed_post_from_dict = ListedPost.from_dict(listed_post_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


