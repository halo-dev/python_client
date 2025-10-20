# LocalThumbnailSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_path** | **str** | Consider the compatibility of the system and migration, use unix-style relative paths  here. | 
**image_signature** | **str** | A hash signature for the image uri. | 
**image_uri** | **str** |  | 
**size** | **str** |  | 
**thumb_signature** | **str** | A hash signature for the thumbnail uri. | 
**thumbnail_uri** | **str** |  | 

## Example

```python
from halo_client.models.local_thumbnail_spec import LocalThumbnailSpec

# TODO update the JSON string below
json = "{}"
# create an instance of LocalThumbnailSpec from a JSON string
local_thumbnail_spec_instance = LocalThumbnailSpec.from_json(json)
# print the JSON string representation of the object
print(LocalThumbnailSpec.to_json())

# convert the object into a dict
local_thumbnail_spec_dict = local_thumbnail_spec_instance.to_dict()
# create an instance of LocalThumbnailSpec from a dict
local_thumbnail_spec_from_dict = LocalThumbnailSpec.from_dict(local_thumbnail_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


