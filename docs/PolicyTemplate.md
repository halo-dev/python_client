# PolicyTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**PolicyTemplateSpec**](PolicyTemplateSpec.md) |  | [optional] 

## Example

```python
from halo_client.models.policy_template import PolicyTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of PolicyTemplate from a JSON string
policy_template_instance = PolicyTemplate.from_json(json)
# print the JSON string representation of the object
print(PolicyTemplate.to_json())

# convert the object into a dict
policy_template_dict = policy_template_instance.to_dict()
# create an instance of PolicyTemplate from a dict
policy_template_from_dict = PolicyTemplate.from_dict(policy_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


