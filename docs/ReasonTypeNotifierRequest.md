# ReasonTypeNotifierRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**notifiers** | **List[str]** |  | [optional] 
**reason_type** | **str** |  | [optional] 

## Example

```python
from halo_client.models.reason_type_notifier_request import ReasonTypeNotifierRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ReasonTypeNotifierRequest from a JSON string
reason_type_notifier_request_instance = ReasonTypeNotifierRequest.from_json(json)
# print the JSON string representation of the object
print(ReasonTypeNotifierRequest.to_json())

# convert the object into a dict
reason_type_notifier_request_dict = reason_type_notifier_request_instance.to_dict()
# create an instance of ReasonTypeNotifierRequest from a dict
reason_type_notifier_request_from_dict = ReasonTypeNotifierRequest.from_dict(reason_type_notifier_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


