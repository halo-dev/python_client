# ContributorVo

A value object for {@link run.halo.app.core.extension.User run.halo.app.core.extension.User}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**avatar** | **str** |  | [optional] 
**bio** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**metadata** | [**Metadata**](Metadata.md) |  | 
**name** | **str** |  | [optional] 
**permalink** | **str** |  | [optional] 

## Example

```python
from halo_client.models.contributor_vo import ContributorVo

# TODO update the JSON string below
json = "{}"
# create an instance of ContributorVo from a JSON string
contributor_vo_instance = ContributorVo.from_json(json)
# print the JSON string representation of the object
print(ContributorVo.to_json())

# convert the object into a dict
contributor_vo_dict = contributor_vo_instance.to_dict()
# create an instance of ContributorVo from a dict
contributor_vo_from_dict = ContributorVo.from_dict(contributor_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


