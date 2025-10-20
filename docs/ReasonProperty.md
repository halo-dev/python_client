# ReasonProperty


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**name** | **str** |  | 
**optional** | **bool** |  | [optional] [default to False]
**type** | **str** |  | 

## Example

```python
from halo_client.models.reason_property import ReasonProperty

# TODO update the JSON string below
json = "{}"
# create an instance of ReasonProperty from a JSON string
reason_property_instance = ReasonProperty.from_json(json)
# print the JSON string representation of the object
print(ReasonProperty.to_json())

# convert the object into a dict
reason_property_dict = reason_property_instance.to_dict()
# create an instance of ReasonProperty from a dict
reason_property_from_dict = ReasonProperty.from_dict(reason_property_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


