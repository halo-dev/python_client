# PostSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**allow_comment** | **bool** |  | [default to True]
**base_snapshot** | **str** |  | [optional] 
**categories** | **List[str]** |  | [optional] 
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
**release_snapshot** | **str** | 文章引用到的已发布的内容，用于主题端显示. | [optional] 
**slug** | **str** |  | 
**tags** | **List[str]** |  | [optional] 
**template** | **str** |  | [optional] 
**title** | **str** |  | 
**visible** | **str** |  | [default to 'PUBLIC']

## Example

```python
from halo_client.models.post_spec import PostSpec

# TODO update the JSON string below
json = "{}"
# create an instance of PostSpec from a JSON string
post_spec_instance = PostSpec.from_json(json)
# print the JSON string representation of the object
print(PostSpec.to_json())

# convert the object into a dict
post_spec_dict = post_spec_instance.to_dict()
# create an instance of PostSpec from a dict
post_spec_from_dict = PostSpec.from_dict(post_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


