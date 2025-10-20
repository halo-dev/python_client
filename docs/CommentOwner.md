# CommentOwner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**annotations** | **Dict[str, str]** |  | [optional] 
**display_name** | **str** |  | [optional] 
**kind** | **str** |  | 
**name** | **str** |  | 

## Example

```python
from halo_client.models.comment_owner import CommentOwner

# TODO update the JSON string below
json = "{}"
# create an instance of CommentOwner from a JSON string
comment_owner_instance = CommentOwner.from_json(json)
# print the JSON string representation of the object
print(CommentOwner.to_json())

# convert the object into a dict
comment_owner_dict = comment_owner_instance.to_dict()
# create an instance of CommentOwner from a dict
comment_owner_from_dict = CommentOwner.from_dict(comment_owner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


