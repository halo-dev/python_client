# Ref

Extension reference object. The name is mandatory

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**group** | **str** | Extension group | 
**kind** | **str** | Extension kind | 
**name** | **str** | Extension name. This field is mandatory | 
**version** | **str** | Extension version | [optional] 

## Example

```python
from halo_client.models.ref import Ref

# TODO update the JSON string below
json = "{}"
# create an instance of Ref from a JSON string
ref_instance = Ref.from_json(json)
# print the JSON string representation of the object
print(Ref.to_json())

# convert the object into a dict
ref_dict = ref_instance.to_dict()
# create an instance of Ref from a dict
ref_from_dict = Ref.from_dict(ref_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


