# ContentUpdateParam


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** |  | 
**raw** | **str** |  | 
**raw_type** | **str** |  | 
**version** | **int** |  | [optional] 

## Example

```python
from halo_client.models.content_update_param import ContentUpdateParam

# TODO update the JSON string below
json = "{}"
# create an instance of ContentUpdateParam from a JSON string
content_update_param_instance = ContentUpdateParam.from_json(json)
# print the JSON string representation of the object
print(ContentUpdateParam.to_json())

# convert the object into a dict
content_update_param_dict = content_update_param_instance.to_dict()
# create an instance of ContentUpdateParam from a dict
content_update_param_from_dict = ContentUpdateParam.from_dict(content_update_param_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


