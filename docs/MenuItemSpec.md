# MenuItemSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**children** | **List[str]** | Children of this menu item | [optional] 
**display_name** | **str** | The display name of menu item. | [optional] 
**href** | **str** | The href of this menu item. | [optional] 
**priority** | **int** | The priority is for ordering. | [optional] 
**target** | **str** | The &lt;a&gt; target attribute of this menu item. | [optional] 
**target_ref** | [**Ref**](Ref.md) |  | [optional] 

## Example

```python
from halo_client.models.menu_item_spec import MenuItemSpec

# TODO update the JSON string below
json = "{}"
# create an instance of MenuItemSpec from a JSON string
menu_item_spec_instance = MenuItemSpec.from_json(json)
# print the JSON string representation of the object
print(MenuItemSpec.to_json())

# convert the object into a dict
menu_item_spec_dict = menu_item_spec_instance.to_dict()
# create an instance of MenuItemSpec from a dict
menu_item_spec_from_dict = MenuItemSpec.from_dict(menu_item_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


