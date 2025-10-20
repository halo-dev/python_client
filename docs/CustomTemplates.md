# CustomTemplates


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category** | [**List[TemplateDescriptor]**](TemplateDescriptor.md) |  | [optional] 
**page** | [**List[TemplateDescriptor]**](TemplateDescriptor.md) |  | [optional] 
**post** | [**List[TemplateDescriptor]**](TemplateDescriptor.md) |  | [optional] 

## Example

```python
from halo_client.models.custom_templates import CustomTemplates

# TODO update the JSON string below
json = "{}"
# create an instance of CustomTemplates from a JSON string
custom_templates_instance = CustomTemplates.from_json(json)
# print the JSON string representation of the object
print(CustomTemplates.to_json())

# convert the object into a dict
custom_templates_dict = custom_templates_instance.to_dict()
# create an instance of CustomTemplates from a dict
custom_templates_from_dict = CustomTemplates.from_dict(custom_templates_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


