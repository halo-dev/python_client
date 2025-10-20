# NotifierDescriptor

<p>{@link NotifierDescriptor NotifierDescriptor} is a custom extension that defines a notifier.</p>  <p>It describes the notifier's name, description, and the extension name of the notifier to  let the user know what the notifier is and what it can do in the UI and also let the  <code>NotificationCenter</code> know how to load the notifier and prepare the notifier's settings.</p>

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**NotifierDescriptorSpec**](NotifierDescriptorSpec.md) |  | [optional] 

## Example

```python
from halo_client.models.notifier_descriptor import NotifierDescriptor

# TODO update the JSON string below
json = "{}"
# create an instance of NotifierDescriptor from a JSON string
notifier_descriptor_instance = NotifierDescriptor.from_json(json)
# print the JSON string representation of the object
print(NotifierDescriptor.to_json())

# convert the object into a dict
notifier_descriptor_dict = notifier_descriptor_instance.to_dict()
# create an instance of NotifierDescriptor from a dict
notifier_descriptor_from_dict = NotifierDescriptor.from_dict(notifier_descriptor_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


