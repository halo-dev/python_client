# TemplateDescriptor

Type used to describe custom template page.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**file** | **str** |  | 
**name** | **str** |  | 
**screenshot** | **str** |  | [optional] 

## Example

```python
from halo_client.models.template_descriptor import TemplateDescriptor

# TODO update the JSON string below
json = "{}"
# create an instance of TemplateDescriptor from a JSON string
template_descriptor_instance = TemplateDescriptor.from_json(json)
# print the JSON string representation of the object
print(TemplateDescriptor.to_json())

# convert the object into a dict
template_descriptor_dict = template_descriptor_instance.to_dict()
# create an instance of TemplateDescriptor from a dict
template_descriptor_from_dict = TemplateDescriptor.from_dict(template_descriptor_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


