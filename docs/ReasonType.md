# ReasonType

<p>{@link ReasonType ReasonType} is a custom extension that defines a type of reason.</p>  <p>One {@link ReasonType ReasonType} can have multiple {@link Reason Reason}s to notify.</p>

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**ReasonTypeSpec**](ReasonTypeSpec.md) |  | [optional] 

## Example

```python
from halo_client.models.reason_type import ReasonType

# TODO update the JSON string below
json = "{}"
# create an instance of ReasonType from a JSON string
reason_type_instance = ReasonType.from_json(json)
# print the JSON string representation of the object
print(ReasonType.to_json())

# convert the object into a dict
reason_type_dict = reason_type_instance.to_dict()
# create an instance of ReasonType from a dict
reason_type_from_dict = ReasonType.from_dict(reason_type_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


