# TemplateContent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**html_body** | **str** |  | [optional] 
**raw_body** | **str** |  | [optional] 
**title** | **str** |  | 

## Example

```python
from halo_client.models.template_content import TemplateContent

# TODO update the JSON string below
json = "{}"
# create an instance of TemplateContent from a JSON string
template_content_instance = TemplateContent.from_json(json)
# print the JSON string representation of the object
print(TemplateContent.to_json())

# convert the object into a dict
template_content_dict = template_content_instance.to_dict()
# create an instance of TemplateContent from a dict
template_content_from_dict = TemplateContent.from_dict(template_content_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


