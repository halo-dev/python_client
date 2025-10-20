# Stats

Stats value object.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**approved_comment** | **int** |  | [optional] 
**total_comment** | **int** |  | [optional] 
**upvote** | **int** |  | [optional] 
**visit** | **int** |  | [optional] 

## Example

```python
from halo_client.models.stats import Stats

# TODO update the JSON string below
json = "{}"
# create an instance of Stats from a JSON string
stats_instance = Stats.from_json(json)
# print the JSON string representation of the object
print(Stats.to_json())

# convert the object into a dict
stats_dict = stats_instance.to_dict()
# create an instance of Stats from a dict
stats_from_dict = Stats.from_dict(stats_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


