# UserConnectionSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**provider_user_id** | **str** | The unique identifier for the user&#39;s connection to the OAuth provider.  for example, the user&#39;s GitHub id. | 
**registration_id** | **str** | The name of the OAuth provider (e.g. Google, Facebook, Twitter). | 
**updated_at** | **datetime** | The time when the user connection was last updated. | [optional] 
**username** | **str** | The {@link Metadata#getName Metadata#getName()} of the user associated with the OAuth connection. | 

## Example

```python
from halo_client.models.user_connection_spec import UserConnectionSpec

# TODO update the JSON string below
json = "{}"
# create an instance of UserConnectionSpec from a JSON string
user_connection_spec_instance = UserConnectionSpec.from_json(json)
# print the JSON string representation of the object
print(UserConnectionSpec.to_json())

# convert the object into a dict
user_connection_spec_dict = user_connection_spec_instance.to_dict()
# create an instance of UserConnectionSpec from a dict
user_connection_spec_from_dict = UserConnectionSpec.from_dict(user_connection_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


