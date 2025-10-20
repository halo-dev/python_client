# UcUploadFromUrlRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**filename** | **str** | Custom file name | [optional] 
**url** | **str** |  | 

## Example

```python
from halo_client.models.uc_upload_from_url_request import UcUploadFromUrlRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UcUploadFromUrlRequest from a JSON string
uc_upload_from_url_request_instance = UcUploadFromUrlRequest.from_json(json)
# print the JSON string representation of the object
print(UcUploadFromUrlRequest.to_json())

# convert the object into a dict
uc_upload_from_url_request_dict = uc_upload_from_url_request_instance.to_dict()
# create an instance of UcUploadFromUrlRequest from a dict
uc_upload_from_url_request_from_dict = UcUploadFromUrlRequest.from_dict(uc_upload_from_url_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


