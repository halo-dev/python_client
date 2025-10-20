# ReplySpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**allow_notification** | **bool** |  | [default to True]
**approved** | **bool** |  | [default to False]
**approved_time** | **datetime** |  | [optional] 
**comment_name** | **str** |  | 
**content** | **str** |  | 
**creation_time** | **datetime** | The user-defined creation time default is &lt;code&gt;metadata.creationTimestamp&lt;/code&gt;. | [optional] 
**hidden** | **bool** |  | [default to False]
**ip_address** | **str** |  | [optional] 
**owner** | [**CommentOwner**](CommentOwner.md) |  | 
**priority** | **int** |  | [default to 0]
**quote_reply** | **str** |  | [optional] 
**raw** | **str** |  | 
**top** | **bool** |  | [default to False]
**user_agent** | **str** |  | [optional] 

## Example

```python
from halo_client.models.reply_spec import ReplySpec

# TODO update the JSON string below
json = "{}"
# create an instance of ReplySpec from a JSON string
reply_spec_instance = ReplySpec.from_json(json)
# print the JSON string representation of the object
print(ReplySpec.to_json())

# convert the object into a dict
reply_spec_dict = reply_spec_instance.to_dict()
# create an instance of ReplySpec from a dict
reply_spec_from_dict = ReplySpec.from_dict(reply_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


