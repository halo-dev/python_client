# ThemeSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**author** | [**Author**](Author.md) |  | 
**config_map_name** | **str** |  | [optional] 
**custom_templates** | [**CustomTemplates**](CustomTemplates.md) |  | [optional] 
**description** | **str** |  | [optional] 
**display_name** | **str** |  | 
**homepage** | **str** |  | [optional] 
**issues** | **str** |  | [optional] 
**license** | [**List[License]**](License.md) |  | [optional] 
**logo** | **str** |  | [optional] 
**repo** | **str** |  | [optional] 
**requires** | **str** |  | [optional] 
**setting_name** | **str** |  | [optional] 
**version** | **str** |  | [optional] 

## Example

```python
from halo_client.models.theme_spec import ThemeSpec

# TODO update the JSON string below
json = "{}"
# create an instance of ThemeSpec from a JSON string
theme_spec_instance = ThemeSpec.from_json(json)
# print the JSON string representation of the object
print(ThemeSpec.to_json())

# convert the object into a dict
theme_spec_dict = theme_spec_instance.to_dict()
# create an instance of ThemeSpec from a dict
theme_spec_from_dict = ThemeSpec.from_dict(theme_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


