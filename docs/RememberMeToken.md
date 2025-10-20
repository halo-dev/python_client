# RememberMeToken


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**RememberMeTokenSpec**](RememberMeTokenSpec.md) |  | 

## Example

```python
from halo_client.models.remember_me_token import RememberMeToken

# TODO update the JSON string below
json = "{}"
# create an instance of RememberMeToken from a JSON string
remember_me_token_instance = RememberMeToken.from_json(json)
# print the JSON string representation of the object
print(RememberMeToken.to_json())

# convert the object into a dict
remember_me_token_dict = remember_me_token_instance.to_dict()
# create an instance of RememberMeToken from a dict
remember_me_token_from_dict = RememberMeToken.from_dict(remember_me_token_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


