# AttachmentStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**permalink** | **str** | Permalink of attachment. If it is in local storage, the public URL will be set. If it is in s3 storage, the Object URL will be set.  | [optional] 
**thumbnails** | **Dict[str, str]** |  | [optional] 

## Example

```python
from halo_client.models.attachment_status import AttachmentStatus

# TODO update the JSON string below
json = "{}"
# create an instance of AttachmentStatus from a JSON string
attachment_status_instance = AttachmentStatus.from_json(json)
# print the JSON string representation of the object
print(AttachmentStatus.to_json())

# convert the object into a dict
attachment_status_dict = attachment_status_instance.to_dict()
# create an instance of AttachmentStatus from a dict
attachment_status_from_dict = AttachmentStatus.from_dict(attachment_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


