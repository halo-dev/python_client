# Condition

EqualsAndHashCode 排除了lastTransitionTime否则失败时，lastTransitionTime 会被更新  导致 equals 为 false，一直被加入队列.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**last_transition_time** | **datetime** | Last time the condition transitioned from one status to another. | 
**message** | **str** | Human-readable message indicating details about last transition.  This may be an empty string. | [optional] 
**reason** | **str** | Unique, one-word, CamelCase reason for the condition&#39;s last transition. | [optional] 
**status** | **str** | Status is the status of the condition. Can be True, False, Unknown. | 
**type** | **str** | type of condition in CamelCase or in foo.example.com/CamelCase.  example: Ready, Initialized.  maxLength: 316. | 

## Example

```python
from halo_client.models.condition import Condition

# TODO update the JSON string below
json = "{}"
# create an instance of Condition from a JSON string
condition_instance = Condition.from_json(json)
# print the JSON string representation of the object
print(Condition.to_json())

# convert the object into a dict
condition_dict = condition_instance.to_dict()
# create an instance of Condition from a dict
condition_from_dict = Condition.from_dict(condition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


