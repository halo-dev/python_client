# TagStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**observed_version** | **int** |  | [optional] 
**permalink** | **str** |  | [optional] 
**post_count** | **int** |  | [optional] 
**visible_post_count** | **int** |  | [optional] 

## Example

```python
from halo_client.models.tag_status import TagStatus

# TODO update the JSON string below
json = "{}"
# create an instance of TagStatus from a JSON string
tag_status_instance = TagStatus.from_json(json)
# print the JSON string representation of the object
print(TagStatus.to_json())

# convert the object into a dict
tag_status_dict = tag_status_instance.to_dict()
# create an instance of TagStatus from a dict
tag_status_from_dict = TagStatus.from_dict(tag_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


