# LoginHistory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**login_at** | **datetime** |  | 
**reason** | **str** |  | [optional] 
**source_ip** | **str** |  | 
**successful** | **bool** |  | 
**user_agent** | **str** |  | 

## Example

```python
from halo_client.models.login_history import LoginHistory

# TODO update the JSON string below
json = "{}"
# create an instance of LoginHistory from a JSON string
login_history_instance = LoginHistory.from_json(json)
# print the JSON string representation of the object
print(LoginHistory.to_json())

# convert the object into a dict
login_history_dict = login_history_instance.to_dict()
# create an instance of LoginHistory from a dict
login_history_from_dict = LoginHistory.from_dict(login_history_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


