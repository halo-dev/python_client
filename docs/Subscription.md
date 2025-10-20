# Subscription

<p>{@link Subscription Subscription} is a custom extension that defines a subscriber to be notified when a  certain {@link Reason Reason} is triggered.</p>  <p>It holds a {@link Subscriber Subscriber} to the user to be notified, a {@link InterestReason InterestReason} to  subscribe to.</p>

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**SubscriptionSpec**](SubscriptionSpec.md) |  | [optional] 

## Example

```python
from halo_client.models.subscription import Subscription

# TODO update the JSON string below
json = "{}"
# create an instance of Subscription from a JSON string
subscription_instance = Subscription.from_json(json)
# print the JSON string representation of the object
print(Subscription.to_json())

# convert the object into a dict
subscription_dict = subscription_instance.to_dict()
# create an instance of Subscription from a dict
subscription_from_dict = Subscription.from_dict(subscription_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


