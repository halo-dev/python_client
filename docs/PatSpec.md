# PatSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**expires_at** | **datetime** |  | [optional] 
**last_used** | **datetime** |  | [optional] 
**name** | **str** |  | 
**revoked** | **bool** |  | [optional] 
**revokes_at** | **datetime** |  | [optional] 
**roles** | **List[str]** |  | [optional] 
**scopes** | **List[str]** |  | [optional] 
**token_id** | **str** |  | 
**username** | **str** |  | 

## Example

```python
from halo_client.models.pat_spec import PatSpec

# TODO update the JSON string below
json = "{}"
# create an instance of PatSpec from a JSON string
pat_spec_instance = PatSpec.from_json(json)
# print the JSON string representation of the object
print(PatSpec.to_json())

# convert the object into a dict
pat_spec_dict = pat_spec_instance.to_dict()
# create an instance of PatSpec from a dict
pat_spec_from_dict = PatSpec.from_dict(pat_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


