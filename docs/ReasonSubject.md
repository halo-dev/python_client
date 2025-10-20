# ReasonSubject


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**name** | **str** |  | 
**title** | **str** |  | 
**url** | **str** |  | [optional] 

## Example

```python
from halo_client.models.reason_subject import ReasonSubject

# TODO update the JSON string below
json = "{}"
# create an instance of ReasonSubject from a JSON string
reason_subject_instance = ReasonSubject.from_json(json)
# print the JSON string representation of the object
print(ReasonSubject.to_json())

# convert the object into a dict
reason_subject_dict = reason_subject_instance.to_dict()
# create an instance of ReasonSubject from a dict
reason_subject_from_dict = ReasonSubject.from_dict(reason_subject_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


