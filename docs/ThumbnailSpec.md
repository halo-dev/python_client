# ThumbnailSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**image_signature** | **str** |  | 
**image_uri** | **str** |  | 
**size** | **str** |  | 
**thumbnail_uri** | **str** |  | 

## Example

```python
from halo_client.models.thumbnail_spec import ThumbnailSpec

# TODO update the JSON string below
json = "{}"
# create an instance of ThumbnailSpec from a JSON string
thumbnail_spec_instance = ThumbnailSpec.from_json(json)
# print the JSON string representation of the object
print(ThumbnailSpec.to_json())

# convert the object into a dict
thumbnail_spec_dict = thumbnail_spec_instance.to_dict()
# create an instance of ThumbnailSpec from a dict
thumbnail_spec_from_dict = ThumbnailSpec.from_dict(thumbnail_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


