# PostVo

A value object for {@link Post Post}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**categories** | [**List[CategoryVo]**](CategoryVo.md) |  | [optional] 
**content** | [**ContentVo**](ContentVo.md) |  | [optional] 
**contributors** | [**List[ContributorVo]**](ContributorVo.md) |  | [optional] 
**metadata** | [**Metadata**](Metadata.md) |  | 
**owner** | [**ContributorVo**](ContributorVo.md) |  | [optional] 
**spec** | [**PostSpec**](PostSpec.md) |  | [optional] 
**stats** | [**StatsVo**](StatsVo.md) |  | [optional] 
**status** | [**PostStatus**](PostStatus.md) |  | [optional] 
**tags** | [**List[TagVo]**](TagVo.md) |  | [optional] 

## Example

```python
from halo_client.models.post_vo import PostVo

# TODO update the JSON string below
json = "{}"
# create an instance of PostVo from a JSON string
post_vo_instance = PostVo.from_json(json)
# print the JSON string representation of the object
print(PostVo.to_json())

# convert the object into a dict
post_vo_dict = post_vo_instance.to_dict()
# create an instance of PostVo from a dict
post_vo_from_dict = PostVo.from_dict(post_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


