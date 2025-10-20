# UploadFromUrlRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**filename** | **str** | Custom file name | [optional] 
**group_name** | **str** | The name of the group to which the attachment belongs | [optional] 
**policy_name** | **str** | Storage policy name | 
**url** | **str** |  | 

## Example

```python
from halo_client.models.upload_from_url_request import UploadFromUrlRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UploadFromUrlRequest from a JSON string
upload_from_url_request_instance = UploadFromUrlRequest.from_json(json)
# print the JSON string representation of the object
print(UploadFromUrlRequest.to_json())

# convert the object into a dict
upload_from_url_request_dict = upload_from_url_request_instance.to_dict()
# create an instance of UploadFromUrlRequest from a dict
upload_from_url_request_from_dict = UploadFromUrlRequest.from_dict(upload_from_url_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


