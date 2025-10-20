# SiteStatsVo

A value object for site stats.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category** | **int** |  | [optional] 
**comment** | **int** |  | [optional] 
**post** | **int** |  | [optional] 
**upvote** | **int** |  | [optional] 
**visit** | **int** |  | [optional] 

## Example

```python
from halo_client.models.site_stats_vo import SiteStatsVo

# TODO update the JSON string below
json = "{}"
# create an instance of SiteStatsVo from a JSON string
site_stats_vo_instance = SiteStatsVo.from_json(json)
# print the JSON string representation of the object
print(SiteStatsVo.to_json())

# convert the object into a dict
site_stats_vo_dict = site_stats_vo_instance.to_dict()
# create an instance of SiteStatsVo from a dict
site_stats_vo_from_dict = SiteStatsVo.from_dict(site_stats_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


