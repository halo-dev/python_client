# CommentRequest

Request parameter object for {@link Comment Comment}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**allow_notification** | **bool** |  | [optional] [default to False]
**content** | **str** |  | 
**hidden** | **bool** |  | [optional] [default to False]
**owner** | [**CommentEmailOwner**](CommentEmailOwner.md) |  | [optional] 
**raw** | **str** |  | 
**subject_ref** | [**Ref**](Ref.md) |  | 

## Example

```python
from halo_client.models.comment_request import CommentRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommentRequest from a JSON string
comment_request_instance = CommentRequest.from_json(json)
# print the JSON string representation of the object
print(CommentRequest.to_json())

# convert the object into a dict
comment_request_dict = comment_request_instance.to_dict()
# create an instance of CommentRequest from a dict
comment_request_from_dict = CommentRequest.from_dict(comment_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


