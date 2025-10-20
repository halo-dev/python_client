# SearchOption

Search option. It is used to control search behavior.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**annotations** | **Dict[str, str]** | Additional annotations for extending search option by other search engines. | [optional] 
**filter_exposed** | **bool** | Whether to filter exposed content. If null, it will not filter. | [optional] 
**filter_published** | **bool** | Whether to filter published content. If null, it will not filter. | [optional] 
**filter_recycled** | **bool** | Whether to filter recycled content. If null, it will not filter. | [optional] 
**highlight_post_tag** | **str** | Post HTML tag of highlighted fragment. | [optional] 
**highlight_pre_tag** | **str** | Pre HTML tag of highlighted fragment. | [optional] 
**include_category_names** | **List[str]** | Category names to include(and). If null, it will include all categories. | [optional] 
**include_owner_names** | **List[str]** | Owner names to include(or). If null, it will include all owners. | [optional] 
**include_tag_names** | **List[str]** | Tag names to include(and). If null, it will include all tags. | [optional] 
**include_types** | **List[str]** | Types to include(or). If null, it will include all types. | [optional] 
**keyword** | **str** | Search keyword. | 
**limit** | **int** | Limit of result. | [optional] 

## Example

```python
from halo_client.models.search_option import SearchOption

# TODO update the JSON string below
json = "{}"
# create an instance of SearchOption from a JSON string
search_option_instance = SearchOption.from_json(json)
# print the JSON string representation of the object
print(SearchOption.to_json())

# convert the object into a dict
search_option_dict = search_option_instance.to_dict()
# create an instance of SearchOption from a dict
search_option_from_dict = SearchOption.from_dict(search_option_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


