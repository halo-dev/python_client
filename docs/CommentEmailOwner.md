# CommentEmailOwner

<p>The creator info of the comment.</p>  This {@link CommentEmailOwner CommentEmailOwner} is only applicable to the user who is allowed to comment  without logging in.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**avatar** | **str** | avatar for comment owner | [optional] 
**display_name** | **str** | display name for comment owner | [optional] 
**email** | **str** | email for comment owner | [optional] 
**website** | **str** | website for comment owner | [optional] 

## Example

```python
from halo_client.models.comment_email_owner import CommentEmailOwner

# TODO update the JSON string below
json = "{}"
# create an instance of CommentEmailOwner from a JSON string
comment_email_owner_instance = CommentEmailOwner.from_json(json)
# print the JSON string representation of the object
print(CommentEmailOwner.to_json())

# convert the object into a dict
comment_email_owner_dict = comment_email_owner_instance.to_dict()
# create an instance of CommentEmailOwner from a dict
comment_email_owner_from_dict = CommentEmailOwner.from_dict(comment_email_owner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


