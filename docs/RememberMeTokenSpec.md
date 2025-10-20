# RememberMeTokenSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**last_used** | **datetime** |  | [optional] 
**series** | **str** |  | 
**token_value** | **str** |  | 
**username** | **str** |  | 

## Example

```python
from halo_client.models.remember_me_token_spec import RememberMeTokenSpec

# TODO update the JSON string below
json = "{}"
# create an instance of RememberMeTokenSpec from a JSON string
remember_me_token_spec_instance = RememberMeTokenSpec.from_json(json)
# print the JSON string representation of the object
print(RememberMeTokenSpec.to_json())

# convert the object into a dict
remember_me_token_spec_dict = remember_me_token_spec_instance.to_dict()
# create an instance of RememberMeTokenSpec from a dict
remember_me_token_spec_from_dict = RememberMeTokenSpec.from_dict(remember_me_token_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


