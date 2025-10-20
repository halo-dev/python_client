# SinglePageVo

A value object for {@link SinglePage SinglePage}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | [**ContentVo**](ContentVo.md) |  | [optional] 
**contributors** | [**List[ContributorVo]**](ContributorVo.md) |  | [optional] 
**metadata** | [**Metadata**](Metadata.md) |  | 
**owner** | [**ContributorVo**](ContributorVo.md) |  | [optional] 
**spec** | [**SinglePageSpec**](SinglePageSpec.md) |  | [optional] 
**stats** | [**StatsVo**](StatsVo.md) |  | [optional] 
**status** | [**SinglePageStatus**](SinglePageStatus.md) |  | [optional] 

## Example

```python
from halo_client.models.single_page_vo import SinglePageVo

# TODO update the JSON string below
json = "{}"
# create an instance of SinglePageVo from a JSON string
single_page_vo_instance = SinglePageVo.from_json(json)
# print the JSON string representation of the object
print(SinglePageVo.to_json())

# convert the object into a dict
single_page_vo_dict = single_page_vo_instance.to_dict()
# create an instance of SinglePageVo from a dict
single_page_vo_from_dict = SinglePageVo.from_dict(single_page_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


