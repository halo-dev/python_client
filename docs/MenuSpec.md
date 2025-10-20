# MenuSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** | The display name of the menu. | 
**menu_items** | **List[str]** | Menu items of this menu. | [optional] 

## Example

```python
from halo_client.models.menu_spec import MenuSpec

# TODO update the JSON string below
json = "{}"
# create an instance of MenuSpec from a JSON string
menu_spec_instance = MenuSpec.from_json(json)
# print the JSON string representation of the object
print(MenuSpec.to_json())

# convert the object into a dict
menu_spec_dict = menu_spec_instance.to_dict()
# create an instance of MenuSpec from a dict
menu_spec_from_dict = MenuSpec.from_dict(menu_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


