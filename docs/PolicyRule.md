# PolicyRule

PolicyRule holds information that describes a policy rule, but does not contain information  about whom the rule applies to or which namespace the rule applies to.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_groups** | **List[str]** | APIGroups is the name of the APIGroup that contains the resources.  If multiple API groups are specified, any action requested against one of the enumerated  resources in any API group will be allowed. | [optional] 
**non_resource_urls** | **List[str]** | NonResourceURLs is a set of partial urls that a user should have access to.  *s are allowed, but only as the full, final step in the path  If an action is not a resource API request, then the URL is split on &#39;/&#39; and is checked  against the NonResourceURLs to look for a match.  Since non-resource URLs are not namespaced, this field is only applicable for  ClusterRoles referenced from a ClusterRoleBinding.  Rules can either apply to API resources (such as \&quot;pods\&quot; or \&quot;secrets\&quot;) or non-resource  URL paths (such as \&quot;/api\&quot;),  but not both. | [optional] 
**resource_names** | **List[str]** | ResourceNames is an optional white list of names that the rule applies to.  An empty set  means that everything is allowed. | [optional] 
**resources** | **List[str]** | Resources is a list of resources this rule applies to.  &#39;*&#39; represents all resources in  the specified apiGroups.  &#39;*&amp;#47;foo&#39; represents the subresource &#39;foo&#39; for all resources in the specified  apiGroups. | [optional] 
**verbs** | **List[str]** | about who the rule applies to or which namespace the rule applies to. | [optional] 

## Example

```python
from halo_client.models.policy_rule import PolicyRule

# TODO update the JSON string below
json = "{}"
# create an instance of PolicyRule from a JSON string
policy_rule_instance = PolicyRule.from_json(json)
# print the JSON string representation of the object
print(PolicyRule.to_json())

# convert the object into a dict
policy_rule_dict = policy_rule_instance.to_dict()
# create an instance of PolicyRule from a dict
policy_rule_from_dict = PolicyRule.from_dict(policy_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


