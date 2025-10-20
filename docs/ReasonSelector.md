# ReasonSelector


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**language** | **str** |  | [default to 'default']
**reason_type** | **str** |  | 

## Example

```python
from halo_client.models.reason_selector import ReasonSelector

# TODO update the JSON string below
json = "{}"
# create an instance of ReasonSelector from a JSON string
reason_selector_instance = ReasonSelector.from_json(json)
# print the JSON string representation of the object
print(ReasonSelector.to_json())

# convert the object into a dict
reason_selector_dict = reason_selector_instance.to_dict()
# create an instance of ReasonSelector from a dict
reason_selector_from_dict = ReasonSelector.from_dict(reason_selector_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


