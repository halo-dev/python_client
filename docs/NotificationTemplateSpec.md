# NotificationTemplateSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reason_selector** | [**ReasonSelector**](ReasonSelector.md) |  | [optional] 
**template** | [**TemplateContent**](TemplateContent.md) |  | [optional] 

## Example

```python
from halo_client.models.notification_template_spec import NotificationTemplateSpec

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTemplateSpec from a JSON string
notification_template_spec_instance = NotificationTemplateSpec.from_json(json)
# print the JSON string representation of the object
print(NotificationTemplateSpec.to_json())

# convert the object into a dict
notification_template_spec_dict = notification_template_spec_instance.to_dict()
# create an instance of NotificationTemplateSpec from a dict
notification_template_spec_from_dict = NotificationTemplateSpec.from_dict(notification_template_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


