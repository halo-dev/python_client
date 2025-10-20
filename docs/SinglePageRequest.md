# SinglePageRequest

A request parameter for {@link SinglePage SinglePage}.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | [**ContentUpdateParam**](ContentUpdateParam.md) |  | 
**page** | [**SinglePage**](SinglePage.md) |  | 

## Example

```python
from halo_client.models.single_page_request import SinglePageRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SinglePageRequest from a JSON string
single_page_request_instance = SinglePageRequest.from_json(json)
# print the JSON string representation of the object
print(SinglePageRequest.to_json())

# convert the object into a dict
single_page_request_dict = single_page_request_instance.to_dict()
# create an instance of SinglePageRequest from a dict
single_page_request_from_dict = SinglePageRequest.from_dict(single_page_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


