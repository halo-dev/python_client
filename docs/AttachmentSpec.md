# AttachmentSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** | Display name of attachment | [optional] 
**group_name** | **str** | Group name | [optional] 
**media_type** | **str** | Media type of attachment | [optional] 
**owner_name** | **str** | Name of User who uploads the attachment | [optional] 
**policy_name** | **str** | Policy name | [optional] 
**size** | **int** | Size of attachment. Unit is Byte | [optional] 
**tags** | **List[str]** | Tags of attachment | [optional] 

## Example

```python
from halo_client.models.attachment_spec import AttachmentSpec

# TODO update the JSON string below
json = "{}"
# create an instance of AttachmentSpec from a JSON string
attachment_spec_instance = AttachmentSpec.from_json(json)
# print the JSON string representation of the object
print(AttachmentSpec.to_json())

# convert the object into a dict
attachment_spec_dict = attachment_spec_instance.to_dict()
# create an instance of AttachmentSpec from a dict
attachment_spec_from_dict = AttachmentSpec.from_dict(attachment_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


