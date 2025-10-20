# SubscriptionSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**disabled** | **bool** | Perhaps users need to unsubscribe and interact without receiving notifications again | [optional] 
**reason** | [**InterestReason**](InterestReason.md) |  | 
**subscriber** | [**SubscriptionSubscriber**](SubscriptionSubscriber.md) |  | 
**unsubscribe_token** | **str** | The token to unsubscribe | 

## Example

```python
from halo_client.models.subscription_spec import SubscriptionSpec

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionSpec from a JSON string
subscription_spec_instance = SubscriptionSpec.from_json(json)
# print the JSON string representation of the object
print(SubscriptionSpec.to_json())

# convert the object into a dict
subscription_spec_dict = subscription_spec_instance.to_dict()
# create an instance of SubscriptionSpec from a dict
subscription_spec_from_dict = SubscriptionSpec.from_dict(subscription_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


