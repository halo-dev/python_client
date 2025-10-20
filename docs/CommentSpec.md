# CommentSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**allow_notification** | **bool** |  | [default to True]
**approved** | **bool** |  | [default to False]
**approved_time** | **datetime** |  | [optional] 
**content** | **str** |  | 
**creation_time** | **datetime** | The user-defined creation time default is &lt;code&gt;metadata.creationTimestamp&lt;/code&gt;. | [optional] 
**hidden** | **bool** |  | [default to False]
**ip_address** | **str** |  | [optional] 
**last_read_time** | **datetime** |  | [optional] 
**owner** | [**CommentOwner**](CommentOwner.md) |  | 
**priority** | **int** |  | [default to 0]
**raw** | **str** |  | 
**subject_ref** | [**Ref**](Ref.md) |  | 
**top** | **bool** |  | [default to False]
**user_agent** | **str** |  | [optional] 

## Example

```python
from halo_client.models.comment_spec import CommentSpec

# TODO update the JSON string below
json = "{}"
# create an instance of CommentSpec from a JSON string
comment_spec_instance = CommentSpec.from_json(json)
# print the JSON string representation of the object
print(CommentSpec.to_json())

# convert the object into a dict
comment_spec_dict = comment_spec_instance.to_dict()
# create an instance of CommentSpec from a dict
comment_spec_from_dict = CommentSpec.from_dict(comment_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


