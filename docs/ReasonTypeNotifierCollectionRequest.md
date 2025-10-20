# ReasonTypeNotifierCollectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reason_type_notifiers** | [**List[ReasonTypeNotifierRequest]**](ReasonTypeNotifierRequest.md) |  | 

## Example

```python
from halo_client.models.reason_type_notifier_collection_request import ReasonTypeNotifierCollectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ReasonTypeNotifierCollectionRequest from a JSON string
reason_type_notifier_collection_request_instance = ReasonTypeNotifierCollectionRequest.from_json(json)
# print the JSON string representation of the object
print(ReasonTypeNotifierCollectionRequest.to_json())

# convert the object into a dict
reason_type_notifier_collection_request_dict = reason_type_notifier_collection_request_instance.to_dict()
# create an instance of ReasonTypeNotifierCollectionRequest from a dict
reason_type_notifier_collection_request_from_dict = ReasonTypeNotifierCollectionRequest.from_dict(reason_type_notifier_collection_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


