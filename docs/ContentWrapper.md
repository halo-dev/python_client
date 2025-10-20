# ContentWrapper


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** |  | [optional] 
**raw** | **str** |  | [optional] 
**raw_type** | **str** |  | [optional] 
**snapshot_name** | **str** |  | [optional] 

## Example

```python
from halo_client.models.content_wrapper import ContentWrapper

# TODO update the JSON string below
json = "{}"
# create an instance of ContentWrapper from a JSON string
content_wrapper_instance = ContentWrapper.from_json(json)
# print the JSON string representation of the object
print(ContentWrapper.to_json())

# convert the object into a dict
content_wrapper_dict = content_wrapper_instance.to_dict()
# create an instance of ContentWrapper from a dict
content_wrapper_from_dict = ContentWrapper.from_dict(content_wrapper_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


