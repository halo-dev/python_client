# NotifierInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from halo_client.models.notifier_info import NotifierInfo

# TODO update the JSON string below
json = "{}"
# create an instance of NotifierInfo from a JSON string
notifier_info_instance = NotifierInfo.from_json(json)
# print the JSON string representation of the object
print(NotifierInfo.to_json())

# convert the object into a dict
notifier_info_dict = notifier_info_instance.to_dict()
# create an instance of NotifierInfo from a dict
notifier_info_from_dict = NotifierInfo.from_dict(notifier_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


