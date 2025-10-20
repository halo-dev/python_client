# ReplyRequest

A request parameter object for {@link Reply Reply}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**allow_notification** | **bool** |  | [optional] [default to False]
**content** | **str** |  | 
**hidden** | **bool** |  | [optional] [default to False]
**owner** | [**CommentEmailOwner**](CommentEmailOwner.md) |  | [optional] 
**quote_reply** | **str** |  | [optional] 
**raw** | **str** |  | 

## Example

```python
from halo_client.models.reply_request import ReplyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ReplyRequest from a JSON string
reply_request_instance = ReplyRequest.from_json(json)
# print the JSON string representation of the object
print(ReplyRequest.to_json())

# convert the object into a dict
reply_request_dict = reply_request_instance.to_dict()
# create an instance of ReplyRequest from a dict
reply_request_from_dict = ReplyRequest.from_dict(reply_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


