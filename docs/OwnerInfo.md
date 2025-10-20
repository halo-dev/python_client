# OwnerInfo

Comment owner info.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**avatar** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**kind** | **str** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from halo_client.models.owner_info import OwnerInfo

# TODO update the JSON string below
json = "{}"
# create an instance of OwnerInfo from a JSON string
owner_info_instance = OwnerInfo.from_json(json)
# print the JSON string representation of the object
print(OwnerInfo.to_json())

# convert the object into a dict
owner_info_dict = owner_info_instance.to_dict()
# create an instance of OwnerInfo from a dict
owner_info_from_dict = OwnerInfo.from_dict(owner_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


