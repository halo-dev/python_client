# ListedSnapshotDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**ListedSnapshotSpec**](ListedSnapshotSpec.md) |  | 

## Example

```python
from halo_client.models.listed_snapshot_dto import ListedSnapshotDto

# TODO update the JSON string below
json = "{}"
# create an instance of ListedSnapshotDto from a JSON string
listed_snapshot_dto_instance = ListedSnapshotDto.from_json(json)
# print the JSON string representation of the object
print(ListedSnapshotDto.to_json())

# convert the object into a dict
listed_snapshot_dto_dict = listed_snapshot_dto_instance.to_dict()
# create an instance of ListedSnapshotDto from a dict
listed_snapshot_dto_from_dict = ListedSnapshotDto.from_dict(listed_snapshot_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


