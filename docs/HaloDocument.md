# HaloDocument

Document for search.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**annotations** | **Dict[str, str]** | Custom metadata. Make sure the map is serializable. | [optional] 
**categories** | **List[str]** | Document categories. The item in the list is the category metadata name. | [optional] 
**content** | **str** | Document content. Safety content, without HTML tag. | 
**creation_timestamp** | **datetime** | Document creation timestamp. | [optional] 
**description** | **str** | Document description. | [optional] 
**exposed** | **bool** | Whether the document is exposed to the public. | [optional] 
**id** | **str** | Document ID. It should be unique globally. | 
**metadata_name** | **str** | Metadata name of the corresponding extension. | 
**owner_name** | **str** | Document owner metadata name. | 
**permalink** | **str** | Document permalink. | 
**published** | **bool** | Whether the document is published. | [optional] 
**recycled** | **bool** | Whether the document is recycled. | [optional] 
**tags** | **List[str]** | Document tags. The item in the list is the tag metadata name. | [optional] 
**title** | **str** | Document title. | 
**type** | **str** | Document type. e.g.: post.content.halo.run, singlepage.content.halo.run, moment.moment  .halo.run, doc.doc.halo.run. | 
**update_timestamp** | **datetime** | Document update timestamp. | [optional] 

## Example

```python
from halo_client.models.halo_document import HaloDocument

# TODO update the JSON string below
json = "{}"
# create an instance of HaloDocument from a JSON string
halo_document_instance = HaloDocument.from_json(json)
# print the JSON string representation of the object
print(HaloDocument.to_json())

# convert the object into a dict
halo_document_dict = halo_document_instance.to_dict()
# create an instance of HaloDocument from a dict
halo_document_from_dict = HaloDocument.from_dict(halo_document_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


