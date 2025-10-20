# SinglePageSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**allow_comment** | **bool** |  | [default to True]
**base_snapshot** | **str** |  | [optional] 
**cover** | **str** |  | [optional] 
**deleted** | **bool** |  | [default to False]
**excerpt** | [**Excerpt**](Excerpt.md) |  | 
**head_snapshot** | **str** |  | [optional] 
**html_metas** | **List[Dict[str, str]]** |  | [optional] 
**owner** | **str** |  | [optional] 
**pinned** | **bool** |  | [default to False]
**priority** | **int** |  | [default to 0]
**publish** | **bool** |  | [default to False]
**publish_time** | **datetime** |  | [optional] 
**release_snapshot** | **str** | 引用到的已发布的内容，用于主题端显示. | [optional] 
**slug** | **str** |  | 
**template** | **str** |  | [optional] 
**title** | **str** |  | 
**visible** | **str** |  | [default to 'PUBLIC']

## Example

```python
from halo_client.models.single_page_spec import SinglePageSpec

# TODO update the JSON string below
json = "{}"
# create an instance of SinglePageSpec from a JSON string
single_page_spec_instance = SinglePageSpec.from_json(json)
# print the JSON string representation of the object
print(SinglePageSpec.to_json())

# convert the object into a dict
single_page_spec_dict = single_page_spec_instance.to_dict()
# create an instance of SinglePageSpec from a dict
single_page_spec_from_dict = SinglePageSpec.from_dict(single_page_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


