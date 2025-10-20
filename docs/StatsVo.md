# StatsVo

Stats value object.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**comment** | **int** |  | [optional] 
**upvote** | **int** |  | [optional] 
**visit** | **int** |  | [optional] 

## Example

```python
from halo_client.models.stats_vo import StatsVo

# TODO update the JSON string below
json = "{}"
# create an instance of StatsVo from a JSON string
stats_vo_instance = StatsVo.from_json(json)
# print the JSON string representation of the object
print(StatsVo.to_json())

# convert the object into a dict
stats_vo_dict = stats_vo_instance.to_dict()
# create an instance of StatsVo from a dict
stats_vo_from_dict = StatsVo.from_dict(stats_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


