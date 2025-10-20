# NotifierDescriptorSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**display_name** | **str** |  | 
**notifier_ext_name** | **str** |  | 
**receiver_setting_ref** | [**NotifierSettingRef**](NotifierSettingRef.md) |  | [optional] 
**sender_setting_ref** | [**NotifierSettingRef**](NotifierSettingRef.md) |  | [optional] 

## Example

```python
from halo_client.models.notifier_descriptor_spec import NotifierDescriptorSpec

# TODO update the JSON string below
json = "{}"
# create an instance of NotifierDescriptorSpec from a JSON string
notifier_descriptor_spec_instance = NotifierDescriptorSpec.from_json(json)
# print the JSON string representation of the object
print(NotifierDescriptorSpec.to_json())

# convert the object into a dict
notifier_descriptor_spec_dict = notifier_descriptor_spec_instance.to_dict()
# create an instance of NotifierDescriptorSpec from a dict
notifier_descriptor_spec_from_dict = NotifierDescriptorSpec.from_dict(notifier_descriptor_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


