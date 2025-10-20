# RoleBinding

RoleBinding references a role, but does not contain it.  It can reference a Role in the global.  It adds who information via Subjects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**role_ref** | [**RoleRef**](RoleRef.md) |  | [optional] 
**subjects** | [**List[Subject]**](Subject.md) | Subjects holds references to the objects the role applies to. | [optional] 

## Example

```python
from halo_client.models.role_binding import RoleBinding

# TODO update the JSON string below
json = "{}"
# create an instance of RoleBinding from a JSON string
role_binding_instance = RoleBinding.from_json(json)
# print the JSON string representation of the object
print(RoleBinding.to_json())

# convert the object into a dict
role_binding_dict = role_binding_instance.to_dict()
# create an instance of RoleBinding from a dict
role_binding_from_dict = RoleBinding.from_dict(role_binding_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


