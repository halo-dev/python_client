# PolicySpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config_map_name** | **str** | Reference name of ConfigMap extension | [optional] 
**display_name** | **str** | Display name of policy | 
**template_name** | **str** | Reference name of PolicyTemplate | 

## Example

```python
from halo_client.models.policy_spec import PolicySpec

# TODO update the JSON string below
json = "{}"
# create an instance of PolicySpec from a JSON string
policy_spec_instance = PolicySpec.from_json(json)
# print the JSON string representation of the object
print(PolicySpec.to_json())

# convert the object into a dict
policy_spec_dict = policy_spec_instance.to_dict()
# create an instance of PolicySpec from a dict
policy_spec_from_dict = PolicySpec.from_dict(policy_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


