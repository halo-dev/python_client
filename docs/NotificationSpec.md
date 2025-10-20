# NotificationSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**html_content** | **str** |  | 
**last_read_at** | **datetime** |  | [optional] 
**raw_content** | **str** |  | 
**reason** | **str** | The name of reason | 
**recipient** | **str** | The name of user | 
**title** | **str** |  | 
**unread** | **bool** |  | [optional] 

## Example

```python
from halo_client.models.notification_spec import NotificationSpec

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationSpec from a JSON string
notification_spec_instance = NotificationSpec.from_json(json)
# print the JSON string representation of the object
print(NotificationSpec.to_json())

# convert the object into a dict
notification_spec_dict = notification_spec_instance.to_dict()
# create an instance of NotificationSpec from a dict
notification_spec_from_dict = NotificationSpec.from_dict(notification_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


