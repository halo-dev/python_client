# CategoryStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**permalink** | **str** |  | [optional] 
**post_count** | **int** | 包括当前和其下所有层级的文章数量 (depth&#x3D;max). | [optional] 
**visible_post_count** | **int** | 包括当前和其下所有层级的已发布且公开的文章数量 (depth&#x3D;max). | [optional] 

## Example

```python
from halo_client.models.category_status import CategoryStatus

# TODO update the JSON string below
json = "{}"
# create an instance of CategoryStatus from a JSON string
category_status_instance = CategoryStatus.from_json(json)
# print the JSON string representation of the object
print(CategoryStatus.to_json())

# convert the object into a dict
category_status_dict = category_status_instance.to_dict()
# create an instance of CategoryStatus from a dict
category_status_from_dict = CategoryStatus.from_dict(category_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


