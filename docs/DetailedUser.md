# DetailedUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**roles** | [**List[Role]**](Role.md) |  | 
**user** | [**User**](User.md) |  | 

## Example

```python
from halo_client.models.detailed_user import DetailedUser

# TODO update the JSON string below
json = "{}"
# create an instance of DetailedUser from a JSON string
detailed_user_instance = DetailedUser.from_json(json)
# print the JSON string representation of the object
print(DetailedUser.to_json())

# convert the object into a dict
detailed_user_dict = detailed_user_instance.to_dict()
# create an instance of DetailedUser from a dict
detailed_user_from_dict = DetailedUser.from_dict(detailed_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


