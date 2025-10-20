# UcUploadRequestFormData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**all** | **Dict[str, object]** |  | [optional] 
**empty** | **bool** |  | [optional] 

## Example

```python
from halo_client.models.uc_upload_request_form_data import UcUploadRequestFormData

# TODO update the JSON string below
json = "{}"
# create an instance of UcUploadRequestFormData from a JSON string
uc_upload_request_form_data_instance = UcUploadRequestFormData.from_json(json)
# print the JSON string representation of the object
print(UcUploadRequestFormData.to_json())

# convert the object into a dict
uc_upload_request_form_data_dict = uc_upload_request_form_data_instance.to_dict()
# create an instance of UcUploadRequestFormData from a dict
uc_upload_request_form_data_from_dict = UcUploadRequestFormData.from_dict(uc_upload_request_form_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


