# Reply


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**ReplySpec**](ReplySpec.md) |  | 
**status** | [**ReplyStatus**](ReplyStatus.md) |  | 

## Example

```python
from halo_client.models.reply import Reply

# TODO update the JSON string below
json = "{}"
# create an instance of Reply from a JSON string
reply_instance = Reply.from_json(json)
# print the JSON string representation of the object
print(Reply.to_json())

# convert the object into a dict
reply_dict = reply_instance.to_dict()
# create an instance of Reply from a dict
reply_from_dict = Reply.from_dict(reply_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


