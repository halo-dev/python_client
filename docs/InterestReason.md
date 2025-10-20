# InterestReason

The reason to be interested in

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**expression** | **str** | The expression to be interested in | [optional] 
**reason_type** | **str** | The name of the reason definition to be interested in | 
**subject** | [**InterestReasonSubject**](InterestReasonSubject.md) |  | 

## Example

```python
from halo_client.models.interest_reason import InterestReason

# TODO update the JSON string below
json = "{}"
# create an instance of InterestReason from a JSON string
interest_reason_instance = InterestReason.from_json(json)
# print the JSON string representation of the object
print(InterestReason.to_json())

# convert the object into a dict
interest_reason_dict = interest_reason_instance.to_dict()
# create an instance of InterestReason from a dict
interest_reason_from_dict = InterestReason.from_dict(interest_reason_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


