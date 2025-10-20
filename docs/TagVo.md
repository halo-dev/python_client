# TagVo

A value object for {@link Tag Tag}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**Metadata**](Metadata.md) |  | 
**post_count** | **int** |  | [optional] 
**spec** | [**TagSpec**](TagSpec.md) |  | [optional] 
**status** | [**TagStatus**](TagStatus.md) |  | [optional] 

## Example

```python
from halo_client.models.tag_vo import TagVo

# TODO update the JSON string below
json = "{}"
# create an instance of TagVo from a JSON string
tag_vo_instance = TagVo.from_json(json)
# print the JSON string representation of the object
print(TagVo.to_json())

# convert the object into a dict
tag_vo_dict = tag_vo_instance.to_dict()
# create an instance of TagVo from a dict
tag_vo_from_dict = TagVo.from_dict(tag_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


