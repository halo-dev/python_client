# ReasonTypeSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | 
**display_name** | **str** |  | 
**properties** | [**List[ReasonProperty]**](ReasonProperty.md) |  | [optional] 

## Example

```python
from halo_client.models.reason_type_spec import ReasonTypeSpec

# TODO update the JSON string below
json = "{}"
# create an instance of ReasonTypeSpec from a JSON string
reason_type_spec_instance = ReasonTypeSpec.from_json(json)
# print the JSON string representation of the object
print(ReasonTypeSpec.to_json())

# convert the object into a dict
reason_type_spec_dict = reason_type_spec_instance.to_dict()
# create an instance of ReasonTypeSpec from a dict
reason_type_spec_from_dict = ReasonTypeSpec.from_dict(reason_type_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


