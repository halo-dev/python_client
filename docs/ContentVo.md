# ContentVo

A value object for Content from {@link Snapshot Snapshot}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** |  | [optional] 
**raw** | **str** |  | [optional] 

## Example

```python
from halo_client.models.content_vo import ContentVo

# TODO update the JSON string below
json = "{}"
# create an instance of ContentVo from a JSON string
content_vo_instance = ContentVo.from_json(json)
# print the JSON string representation of the object
print(ContentVo.to_json())

# convert the object into a dict
content_vo_dict = content_vo_instance.to_dict()
# create an instance of ContentVo from a dict
content_vo_from_dict = ContentVo.from_dict(content_vo_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


