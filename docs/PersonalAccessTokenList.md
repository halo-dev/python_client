# PersonalAccessTokenList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**first** | **bool** | Indicates whether current page is the first page. | 
**has_next** | **bool** | Indicates whether current page has previous page. | 
**has_previous** | **bool** | Indicates whether current page has previous page. | 
**items** | [**List[PersonalAccessToken]**](PersonalAccessToken.md) | A chunk of items. | 
**last** | **bool** | Indicates whether current page is the last page. | 
**page** | **int** | Page number, starts from 1. If not set or equal to 0, it means no pagination. | 
**size** | **int** | Size of each page. If not set or equal to 0, it means no pagination. | 
**total** | **int** | Total elements. | 
**total_pages** | **int** | Indicates total pages. | 

## Example

```python
from halo_client.models.personal_access_token_list import PersonalAccessTokenList

# TODO update the JSON string below
json = "{}"
# create an instance of PersonalAccessTokenList from a JSON string
personal_access_token_list_instance = PersonalAccessTokenList.from_json(json)
# print the JSON string representation of the object
print(PersonalAccessTokenList.to_json())

# convert the object into a dict
personal_access_token_list_dict = personal_access_token_list_instance.to_dict()
# create an instance of PersonalAccessTokenList from a dict
personal_access_token_list_from_dict = PersonalAccessTokenList.from_dict(personal_access_token_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


