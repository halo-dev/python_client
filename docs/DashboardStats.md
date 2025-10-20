# DashboardStats


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**approved_comments** | **int** |  | [optional] 
**comments** | **int** |  | [optional] 
**posts** | **int** |  | [optional] 
**upvotes** | **int** |  | [optional] 
**users** | **int** |  | [optional] 
**visits** | **int** |  | [optional] 

## Example

```python
from halo_client.models.dashboard_stats import DashboardStats

# TODO update the JSON string below
json = "{}"
# create an instance of DashboardStats from a JSON string
dashboard_stats_instance = DashboardStats.from_json(json)
# print the JSON string representation of the object
print(DashboardStats.to_json())

# convert the object into a dict
dashboard_stats_dict = dashboard_stats_instance.to_dict()
# create an instance of DashboardStats from a dict
dashboard_stats_from_dict = DashboardStats.from_dict(dashboard_stats_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


