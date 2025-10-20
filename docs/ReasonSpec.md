# ReasonSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attributes** | [**ReasonAttributes**](ReasonAttributes.md) |  | [optional] 
**author** | **str** |  | 
**reason_type** | **str** |  | 
**subject** | [**ReasonSubject**](ReasonSubject.md) |  | 

## Example

```python
from halo_client.models.reason_spec import ReasonSpec

# TODO update the JSON string below
json = "{}"
# create an instance of ReasonSpec from a JSON string
reason_spec_instance = ReasonSpec.from_json(json)
# print the JSON string representation of the object
print(ReasonSpec.to_json())

# convert the object into a dict
reason_spec_dict = reason_spec_instance.to_dict()
# create an instance of ReasonSpec from a dict
reason_spec_from_dict = ReasonSpec.from_dict(reason_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


