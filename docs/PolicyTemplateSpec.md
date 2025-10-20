# PolicyTemplateSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** |  | [optional] 
**setting_name** | **str** |  | 

## Example

```python
from halo_client.models.policy_template_spec import PolicyTemplateSpec

# TODO update the JSON string below
json = "{}"
# create an instance of PolicyTemplateSpec from a JSON string
policy_template_spec_instance = PolicyTemplateSpec.from_json(json)
# print the JSON string representation of the object
print(PolicyTemplateSpec.to_json())

# convert the object into a dict
policy_template_spec_dict = policy_template_spec_instance.to_dict()
# create an instance of PolicyTemplateSpec from a dict
policy_template_spec_from_dict = PolicyTemplateSpec.from_dict(policy_template_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


