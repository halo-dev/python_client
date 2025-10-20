# SubscriptionSubscriber

The subscriber to be notified

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 

## Example

```python
from halo_client.models.subscription_subscriber import SubscriptionSubscriber

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionSubscriber from a JSON string
subscription_subscriber_instance = SubscriptionSubscriber.from_json(json)
# print the JSON string representation of the object
print(SubscriptionSubscriber.to_json())

# convert the object into a dict
subscription_subscriber_dict = subscription_subscriber_instance.to_dict()
# create an instance of SubscriptionSubscriber from a dict
subscription_subscriber_from_dict = SubscriptionSubscriber.from_dict(subscription_subscriber_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


