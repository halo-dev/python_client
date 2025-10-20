# ListedPostVo

A value object for {@link Post Post}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**categories** | [**List[CategoryVo]**](CategoryVo.md) |  | [optional] 
**contributors** | [**List[ContributorVo]**](ContributorVo.md) |  | [optional] 
**metadata** | [**Metadata**](Metadata.md) |  | 
**owner** | [**ContributorVo**](ContributorVo.md) |  | [optional] 
**spec** | [**PostSpec**](PostSpec.md) |  | [optional] 
**stats** | [**StatsVo**](StatsVo.md) |  | [optional] 
**status** | [**PostStatus**](PostStatus.md) |  | [optional] 
**tags** | [**List[TagVo]**](TagVo.md) |  | [optional] 

## Example

```python
from halo_client.models.listed_post_vo import ListedPostVo

# TODO update the JSON string below
json = "{}"
# create an instance of ListedPostVo from a JSON string
listed_post_vo_instance = ListedPostVo.from_json(json)
# print the JSON string representation of the object
print(ListedPostVo.to_json())

# convert the object into a dict
listed_post_vo_dict = listed_post_vo_instance.to_dict()
# create an instance of ListedPostVo from a dict
listed_post_vo_from_dict = ListedPostVo.from_dict(listed_post_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


