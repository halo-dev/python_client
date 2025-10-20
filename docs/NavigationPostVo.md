# NavigationPostVo

Post navigation vo to hold previous and next item.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current** | [**PostVo**](PostVo.md) |  | [optional] 
**next** | [**PostVo**](PostVo.md) |  | [optional] 
**previous** | [**PostVo**](PostVo.md) |  | [optional] 

## Example

```python
from halo_client.models.navigation_post_vo import NavigationPostVo

# TODO update the JSON string below
json = "{}"
# create an instance of NavigationPostVo from a JSON string
navigation_post_vo_instance = NavigationPostVo.from_json(json)
# print the JSON string representation of the object
print(NavigationPostVo.to_json())

# convert the object into a dict
navigation_post_vo_dict = navigation_post_vo_instance.to_dict()
# create an instance of NavigationPostVo from a dict
navigation_post_vo_from_dict = NavigationPostVo.from_dict(navigation_post_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


