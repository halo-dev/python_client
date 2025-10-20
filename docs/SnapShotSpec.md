# SnapShotSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content_patch** | **str** |  | [optional] 
**contributors** | **List[str]** |  | [optional] 
**last_modify_time** | **datetime** |  | [optional] 
**owner** | **str** |  | 
**parent_snapshot_name** | **str** |  | [optional] 
**raw_patch** | **str** |  | [optional] 
**raw_type** | **str** | such as: markdown | html | json | asciidoc | latex. | 
**subject_ref** | [**Ref**](Ref.md) |  | 

## Example

```python
from halo_client.models.snap_shot_spec import SnapShotSpec

# TODO update the JSON string below
json = "{}"
# create an instance of SnapShotSpec from a JSON string
snap_shot_spec_instance = SnapShotSpec.from_json(json)
# print the JSON string representation of the object
print(SnapShotSpec.to_json())

# convert the object into a dict
snap_shot_spec_dict = snap_shot_spec_instance.to_dict()
# create an instance of SnapShotSpec from a dict
snap_shot_spec_from_dict = SnapShotSpec.from_dict(snap_shot_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


