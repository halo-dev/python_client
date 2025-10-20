# Notification

<p>{@link Notification Notification} is a custom extension that used to store notification information for  inner use, it's on-site notification.</p>   <p>Supports the following operations:</p>  <ul>     <li>Marked as read: {@link NotificationSpec#setUnread(boolean) NotificationSpec#setUnread(boolean)}</li>     <li>Get the last read time: {@link NotificationSpec#getLastReadAt NotificationSpec#getLastReadAt()}</li>     <li>Filter by recipient: {@link NotificationSpec#getRecipient NotificationSpec#getRecipient()}</li>  </ul>

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**NotificationSpec**](NotificationSpec.md) |  | [optional] 

## Example

```python
from halo_client.models.notification import Notification

# TODO update the JSON string below
json = "{}"
# create an instance of Notification from a JSON string
notification_instance = Notification.from_json(json)
# print the JSON string representation of the object
print(Notification.to_json())

# convert the object into a dict
notification_dict = notification_instance.to_dict()
# create an instance of Notification from a dict
notification_from_dict = Notification.from_dict(notification_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


