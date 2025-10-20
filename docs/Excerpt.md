# Excerpt


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**auto_generate** | **bool** |  | [default to True]
**raw** | **str** |  | [optional] 

## Example

```python
from halo_client.models.excerpt import Excerpt

# TODO update the JSON string below
json = "{}"
# create an instance of Excerpt from a JSON string
excerpt_instance = Excerpt.from_json(json)
# print the JSON string representation of the object
print(Excerpt.to_json())

# convert the object into a dict
excerpt_dict = excerpt_instance.to_dict()
# create an instance of Excerpt from a dict
excerpt_from_dict = Excerpt.from_dict(excerpt_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


