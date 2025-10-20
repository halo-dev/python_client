# PersonalAccessToken


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**PatSpec**](PatSpec.md) |  | [optional] 

## Example

```python
from halo_client.models.personal_access_token import PersonalAccessToken

# TODO update the JSON string below
json = "{}"
# create an instance of PersonalAccessToken from a JSON string
personal_access_token_instance = PersonalAccessToken.from_json(json)
# print the JSON string representation of the object
print(PersonalAccessToken.to_json())

# convert the object into a dict
personal_access_token_dict = personal_access_token_instance.to_dict()
# create an instance of PersonalAccessToken from a dict
personal_access_token_from_dict = PersonalAccessToken.from_dict(personal_access_token_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


