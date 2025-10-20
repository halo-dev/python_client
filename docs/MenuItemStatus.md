# MenuItemStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** | Calculated Display name of menu item. | [optional] 
**href** | **str** | Calculated href of manu item. | [optional] 

## Example

```python
from halo_client.models.menu_item_status import MenuItemStatus

# TODO update the JSON string below
json = "{}"
# create an instance of MenuItemStatus from a JSON string
menu_item_status_instance = MenuItemStatus.from_json(json)
# print the JSON string representation of the object
print(MenuItemStatus.to_json())

# convert the object into a dict
menu_item_status_dict = menu_item_status_instance.to_dict()
# create an instance of MenuItemStatus from a dict
menu_item_status_from_dict = MenuItemStatus.from_dict(menu_item_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


