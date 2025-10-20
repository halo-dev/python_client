# CounterRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**group** | **str** |  | [optional] 
**hostname** | **str** |  | [optional] 
**language** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**plural** | **str** |  | [optional] 
**referrer** | **str** |  | [optional] 
**screen** | **str** |  | [optional] 

## Example

```python
from halo_client.models.counter_request import CounterRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CounterRequest from a JSON string
counter_request_instance = CounterRequest.from_json(json)
# print the JSON string representation of the object
print(CounterRequest.to_json())

# convert the object into a dict
counter_request_dict = counter_request_instance.to_dict()
# create an instance of CounterRequest from a dict
counter_request_from_dict = CounterRequest.from_dict(counter_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


