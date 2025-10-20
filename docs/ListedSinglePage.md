# ListedSinglePage

A chunk of items.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contributors** | [**List[Contributor]**](Contributor.md) |  | 
**owner** | [**Contributor**](Contributor.md) |  | 
**page** | [**SinglePage**](SinglePage.md) |  | 
**stats** | [**Stats**](Stats.md) |  | 

## Example

```python
from halo_client.models.listed_single_page import ListedSinglePage

# TODO update the JSON string below
json = "{}"
# create an instance of ListedSinglePage from a JSON string
listed_single_page_instance = ListedSinglePage.from_json(json)
# print the JSON string representation of the object
print(ListedSinglePage.to_json())

# convert the object into a dict
listed_single_page_dict = listed_single_page_instance.to_dict()
# create an instance of ListedSinglePage from a dict
listed_single_page_from_dict = ListedSinglePage.from_dict(listed_single_page_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


