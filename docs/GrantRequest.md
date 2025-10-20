# GrantRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**roles** | **List[str]** |  | [optional] 

## Example

```python
from halo_client.models.grant_request import GrantRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GrantRequest from a JSON string
grant_request_instance = GrantRequest.from_json(json)
# print the JSON string representation of the object
print(GrantRequest.to_json())

# convert the object into a dict
grant_request_dict = grant_request_instance.to_dict()
# create an instance of GrantRequest from a dict
grant_request_from_dict = GrantRequest.from_dict(grant_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


