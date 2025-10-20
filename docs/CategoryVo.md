# CategoryVo

A value object for {@link Category Category}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**Metadata**](Metadata.md) |  | 
**post_count** | **int** |  | [optional] 
**spec** | [**CategorySpec**](CategorySpec.md) |  | [optional] 
**status** | [**CategoryStatus**](CategoryStatus.md) |  | [optional] 

## Example

```python
from halo_client.models.category_vo import CategoryVo

# TODO update the JSON string below
json = "{}"
# create an instance of CategoryVo from a JSON string
category_vo_instance = CategoryVo.from_json(json)
# print the JSON string representation of the object
print(CategoryVo.to_json())

# convert the object into a dict
category_vo_dict = category_vo_instance.to_dict()
# create an instance of CategoryVo from a dict
category_vo_from_dict = CategoryVo.from_dict(category_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


