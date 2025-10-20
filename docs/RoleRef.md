# RoleRef

RoleRef contains information that points to the role being used.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_group** | **str** | APIGroup is the group for the resource being referenced. | [optional] 
**kind** | **str** | Kind is the type of resource being referenced. | [optional] 
**name** | **str** | Name is the name of resource being referenced. | [optional] 

## Example

```python
from halo_client.models.role_ref import RoleRef

# TODO update the JSON string below
json = "{}"
# create an instance of RoleRef from a JSON string
role_ref_instance = RoleRef.from_json(json)
# print the JSON string representation of the object
print(RoleRef.to_json())

# convert the object into a dict
role_ref_dict = role_ref_instance.to_dict()
# create an instance of RoleRef from a dict
role_ref_from_dict = RoleRef.from_dict(role_ref_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


