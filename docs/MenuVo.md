# MenuVo

A value object for {@link Menu Menu}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**menu_items** | [**List[MenuItemVo]**](MenuItemVo.md) |  | [optional] 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**MenuSpec**](MenuSpec.md) |  | [optional] 

## Example

```python
from halo_client.models.menu_vo import MenuVo

# TODO update the JSON string below
json = "{}"
# create an instance of MenuVo from a JSON string
menu_vo_instance = MenuVo.from_json(json)
# print the JSON string representation of the object
print(MenuVo.to_json())

# convert the object into a dict
menu_vo_dict = menu_vo_instance.to_dict()
# create an instance of MenuVo from a dict
menu_vo_from_dict = MenuVo.from_dict(menu_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


