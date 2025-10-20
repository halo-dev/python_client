# Subject


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_group** | **str** | APIGroup holds the API group of the referenced subject.  Defaults to \&quot;\&quot; for ServiceAccount subjects.  Defaults to \&quot;rbac.authorization.halo.run\&quot; for User and Group subjects. | [optional] 
**kind** | **str** | Kind of object being referenced. Values defined by this API group are \&quot;User\&quot;, \&quot;Group\&quot;,  and \&quot;ServiceAccount\&quot;.  If the Authorizer does not recognize the kind value, the Authorizer should report  an error. | [optional] 
**name** | **str** | Name of the object being referenced. | [optional] 

## Example

```python
from halo_client.models.subject import Subject

# TODO update the JSON string below
json = "{}"
# create an instance of Subject from a JSON string
subject_instance = Subject.from_json(json)
# print the JSON string representation of the object
print(Subject.to_json())

# convert the object into a dict
subject_dict = subject_instance.to_dict()
# create an instance of Subject from a dict
subject_from_dict = Subject.from_dict(subject_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


