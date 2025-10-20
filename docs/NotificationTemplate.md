# NotificationTemplate

<p>{@link NotificationTemplate NotificationTemplate} is a custom extension that defines a notification template.</p>  <p>It describes the notification template's name, description, and the template content.</p>  <p>{@link Spec#getReasonSelector Spec#getReasonSelector()} is used to select the template by reasonType and language,  if multiple templates are matched, the best match will be selected. This is useful when you  want to override the default template.</p>

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**NotificationTemplateSpec**](NotificationTemplateSpec.md) |  | [optional] 

## Example

```python
from halo_client.models.notification_template import NotificationTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationTemplate from a JSON string
notification_template_instance = NotificationTemplate.from_json(json)
# print the JSON string representation of the object
print(NotificationTemplate.to_json())

# convert the object into a dict
notification_template_dict = notification_template_instance.to_dict()
# create an instance of NotificationTemplate from a dict
notification_template_from_dict = NotificationTemplate.from_dict(notification_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


