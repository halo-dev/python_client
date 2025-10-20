# TagSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**color** | **str** | Color regex explanation.  &lt;pre&gt;  ^                 # start of the line  #                 # start with a number sign &#x60;#&#x60;  (                 # start of (group 1)    [a-fA-F0-9]{6}  # support z-f, A-F and 0-9, with a length of 6    |               # or    [a-fA-F0-9]{3}  # support z-f, A-F and 0-9, with a length of 3  )                 # end of (group 1)  $                 # end of the line  &lt;/pre&gt; | [optional] 
**cover** | **str** |  | [optional] 
**display_name** | **str** |  | 
**slug** | **str** |  | 

## Example

```python
from halo_client.models.tag_spec import TagSpec

# TODO update the JSON string below
json = "{}"
# create an instance of TagSpec from a JSON string
tag_spec_instance = TagSpec.from_json(json)
# print the JSON string representation of the object
print(TagSpec.to_json())

# convert the object into a dict
tag_spec_dict = tag_spec_instance.to_dict()
# create an instance of TagSpec from a dict
tag_spec_from_dict = TagSpec.from_dict(tag_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


