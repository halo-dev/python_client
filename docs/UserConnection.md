# UserConnection

User connection extension.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**UserConnectionSpec**](UserConnectionSpec.md) |  | 

## Example

```python
from halo_client.models.user_connection import UserConnection

# TODO update the JSON string below
json = "{}"
# create an instance of UserConnection from a JSON string
user_connection_instance = UserConnection.from_json(json)
# print the JSON string representation of the object
print(UserConnection.to_json())

# convert the object into a dict
user_connection_dict = user_connection_instance.to_dict()
# create an instance of UserConnection from a dict
user_connection_from_dict = UserConnection.from_dict(user_connection_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


