# Counter

A counter for number of requests by extension resource name.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**approved_comment** | **int** |  | [optional] 
**downvote** | **int** |  | [optional] 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**total_comment** | **int** |  | [optional] 
**upvote** | **int** |  | [optional] 
**visit** | **int** |  | [optional] 

## Example

```python
from halo_client.models.counter import Counter

# TODO update the JSON string below
json = "{}"
# create an instance of Counter from a JSON string
counter_instance = Counter.from_json(json)
# print the JSON string representation of the object
print(Counter.to_json())

# convert the object into a dict
counter_dict = counter_instance.to_dict()
# create an instance of Counter from a dict
counter_from_dict = Counter.from_dict(counter_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


