# Reason

<p>{@link Reason Reason} is a custom extension that defines a reason for a notification, It represents  an instance of a {@link ReasonType ReasonType}.</p>  <p>It can be understood as an event that triggers a notification.</p>

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**ReasonSpec**](ReasonSpec.md) |  | [optional] 

## Example

```python
from halo_client.models.reason import Reason

# TODO update the JSON string below
json = "{}"
# create an instance of Reason from a JSON string
reason_instance = Reason.from_json(json)
# print the JSON string representation of the object
print(Reason.to_json())

# convert the object into a dict
reason_dict = reason_instance.to_dict()
# create an instance of Reason from a dict
reason_from_dict = Reason.from_dict(reason_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


