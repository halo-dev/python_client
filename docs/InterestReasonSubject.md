# InterestReasonSubject

The subject name of reason type to be interested in

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**name** | **str** | if name is not specified, it presents all subjects of the specified reason type and custom resources | [optional] 

## Example

```python
from halo_client.models.interest_reason_subject import InterestReasonSubject

# TODO update the JSON string below
json = "{}"
# create an instance of InterestReasonSubject from a JSON string
interest_reason_subject_instance = InterestReasonSubject.from_json(json)
# print the JSON string representation of the object
print(InterestReasonSubject.to_json())

# convert the object into a dict
interest_reason_subject_dict = interest_reason_subject_instance.to_dict()
# create an instance of InterestReasonSubject from a dict
interest_reason_subject_from_dict = InterestReasonSubject.from_dict(interest_reason_subject_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


