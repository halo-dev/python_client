# ListedSinglePageVo

A chunk of items.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contributors** | [**List[ContributorVo]**](ContributorVo.md) |  | [optional] 
**metadata** | [**Metadata**](Metadata.md) |  | 
**owner** | [**ContributorVo**](ContributorVo.md) |  | [optional] 
**spec** | [**SinglePageSpec**](SinglePageSpec.md) |  | [optional] 
**stats** | [**StatsVo**](StatsVo.md) |  | [optional] 
**status** | [**SinglePageStatus**](SinglePageStatus.md) |  | [optional] 

## Example

```python
from halo_client.models.listed_single_page_vo import ListedSinglePageVo

# TODO update the JSON string below
json = "{}"
# create an instance of ListedSinglePageVo from a JSON string
listed_single_page_vo_instance = ListedSinglePageVo.from_json(json)
# print the JSON string representation of the object
print(ListedSinglePageVo.to_json())

# convert the object into a dict
listed_single_page_vo_dict = listed_single_page_vo_instance.to_dict()
# create an instance of ListedSinglePageVo from a dict
listed_single_page_vo_from_dict = ListedSinglePageVo.from_dict(listed_single_page_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


