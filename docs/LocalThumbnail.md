# LocalThumbnail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**LocalThumbnailSpec**](LocalThumbnailSpec.md) |  | 
**status** | [**LocalThumbnailStatus**](LocalThumbnailStatus.md) |  | 

## Example

```python
from halo_client.models.local_thumbnail import LocalThumbnail

# TODO update the JSON string below
json = "{}"
# create an instance of LocalThumbnail from a JSON string
local_thumbnail_instance = LocalThumbnail.from_json(json)
# print the JSON string representation of the object
print(LocalThumbnail.to_json())

# convert the object into a dict
local_thumbnail_dict = local_thumbnail_instance.to_dict()
# create an instance of LocalThumbnail from a dict
local_thumbnail_from_dict = LocalThumbnail.from_dict(local_thumbnail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


