# SinglePage

<p>Single page extension.</p>

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**SinglePageSpec**](SinglePageSpec.md) |  | 
**status** | [**SinglePageStatus**](SinglePageStatus.md) |  | [optional] 

## Example

```python
from halo_client.models.single_page import SinglePage

# TODO update the JSON string below
json = "{}"
# create an instance of SinglePage from a JSON string
single_page_instance = SinglePage.from_json(json)
# print the JSON string representation of the object
print(SinglePage.to_json())

# convert the object into a dict
single_page_dict = single_page_instance.to_dict()
# create an instance of SinglePage from a dict
single_page_from_dict = SinglePage.from_dict(single_page_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


