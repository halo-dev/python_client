# ListedUser

A chunk of items.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**roles** | [**List[Role]**](Role.md) |  | 
**user** | [**User**](User.md) |  | 

## Example

```python
from halo_client.models.listed_user import ListedUser

# TODO update the JSON string below
json = "{}"
# create an instance of ListedUser from a JSON string
listed_user_instance = ListedUser.from_json(json)
# print the JSON string representation of the object
print(ListedUser.to_json())

# convert the object into a dict
listed_user_dict = listed_user_instance.to_dict()
# create an instance of ListedUser from a dict
listed_user_from_dict = ListedUser.from_dict(listed_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


