# ListedSnapshotSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**modify_time** | **datetime** |  | [optional] 
**owner** | **str** |  | 

## Example

```python
from halo_client.models.listed_snapshot_spec import ListedSnapshotSpec

# TODO update the JSON string below
json = "{}"
# create an instance of ListedSnapshotSpec from a JSON string
listed_snapshot_spec_instance = ListedSnapshotSpec.from_json(json)
# print the JSON string representation of the object
print(ListedSnapshotSpec.to_json())

# convert the object into a dict
listed_snapshot_spec_dict = listed_snapshot_spec_instance.to_dict()
# create an instance of ListedSnapshotSpec from a dict
listed_snapshot_spec_from_dict = ListedSnapshotSpec.from_dict(listed_snapshot_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


