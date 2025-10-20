# ThemeStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conditions** | [**List[Condition]**](Condition.md) |  | [optional] 
**location** | **str** |  | [optional] 
**phase** | **str** |  | [optional] 

## Example

```python
from halo_client.models.theme_status import ThemeStatus

# TODO update the JSON string below
json = "{}"
# create an instance of ThemeStatus from a JSON string
theme_status_instance = ThemeStatus.from_json(json)
# print the JSON string representation of the object
print(ThemeStatus.to_json())

# convert the object into a dict
theme_status_dict = theme_status_instance.to_dict()
# create an instance of ThemeStatus from a dict
theme_status_from_dict = ThemeStatus.from_dict(theme_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


