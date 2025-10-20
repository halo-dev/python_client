# MenuItemVo

A value object for {@link MenuItem MenuItem}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** | Gets menu item&#39;s display name. | [optional] 
**metadata** | [**Metadata**](Metadata.md) |  | 
**parent_name** | **str** |  | [optional] 
**spec** | [**MenuItemSpec**](MenuItemSpec.md) |  | [optional] 
**status** | [**MenuItemStatus**](MenuItemStatus.md) |  | [optional] 

## Example

```python
from halo_client.models.menu_item_vo import MenuItemVo

# TODO update the JSON string below
json = "{}"
# create an instance of MenuItemVo from a JSON string
menu_item_vo_instance = MenuItemVo.from_json(json)
# print the JSON string representation of the object
print(MenuItemVo.to_json())

# convert the object into a dict
menu_item_vo_dict = menu_item_vo_instance.to_dict()
# create an instance of MenuItemVo from a dict
menu_item_vo_from_dict = MenuItemVo.from_dict(menu_item_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


