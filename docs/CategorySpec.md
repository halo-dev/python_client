# CategorySpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**children** | **List[str]** |  | [optional] 
**cover** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**display_name** | **str** |  | 
**hide_from_list** | **bool** | &lt;p&gt;Whether to hide the category from the category list.&lt;/p&gt;  &lt;p&gt;When set to true, the category including its subcategories and related posts will  not be displayed in the category list, but it can still be accessed by permalink.&lt;/p&gt;  &lt;p&gt;Limitation: It only takes effect on the theme-side categorized list and it only  allows to be set to true on the first level(root node) of categories.&lt;/p&gt; | [optional] 
**post_template** | **str** | &lt;p&gt;Used to specify the template for the posts associated with the category.&lt;/p&gt;  &lt;p&gt;The priority is not as high as that of the post.&lt;/p&gt;  &lt;p&gt;If the post also specifies a template, the post&#39;s template will prevail.&lt;/p&gt; | [optional] 
**prevent_parent_post_cascade_query** | **bool** | &lt;p&gt;if a category is queried for related posts, the default behavior is to  query all posts under the category including its subcategories, but if this field is  set to true, cascade query behavior will be terminated here.&lt;/p&gt;  &lt;p&gt;For example, if a category has subcategories A and B, and A has subcategories C and  D and C marked this field as true, when querying posts under A category,all posts under A  and B will be queried, but C and D will not be queried.&lt;/p&gt; | [optional] 
**priority** | **int** |  | [default to 0]
**slug** | **str** |  | 
**template** | **str** |  | [optional] 

## Example

```python
from halo_client.models.category_spec import CategorySpec

# TODO update the JSON string below
json = "{}"
# create an instance of CategorySpec from a JSON string
category_spec_instance = CategorySpec.from_json(json)
# print the JSON string representation of the object
print(CategorySpec.to_json())

# convert the object into a dict
category_spec_dict = category_spec_instance.to_dict()
# create an instance of CategorySpec from a dict
category_spec_from_dict = CategorySpec.from_dict(category_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


