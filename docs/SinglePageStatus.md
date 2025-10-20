# SinglePageStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**comments_count** | **int** |  | [optional] 
**conditions** | [**List[Condition]**](Condition.md) |  | [optional] 
**contributors** | **List[str]** |  | [optional] 
**excerpt** | **str** |  | [optional] 
**hide_from_list** | **bool** | see {@link Category.CategorySpec#isHideFromList Category.CategorySpec#isHideFromList()}. | [optional] 
**in_progress** | **bool** |  | [optional] 
**last_modify_time** | **datetime** |  | [optional] 
**observed_version** | **int** |  | [optional] 
**permalink** | **str** |  | [optional] 
**phase** | **str** |  | [optional] 

## Example

```python
from halo_client.models.single_page_status import SinglePageStatus

# TODO update the JSON string below
json = "{}"
# create an instance of SinglePageStatus from a JSON string
single_page_status_instance = SinglePageStatus.from_json(json)
# print the JSON string representation of the object
print(SinglePageStatus.to_json())

# convert the object into a dict
single_page_status_dict = single_page_status_instance.to_dict()
# create an instance of SinglePageStatus from a dict
single_page_status_from_dict = SinglePageStatus.from_dict(single_page_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


