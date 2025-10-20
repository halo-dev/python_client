# BackupSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**expires_at** | **datetime** |  | [optional] 
**format** | **str** | Backup file format. Currently, only zip format is supported. | [optional] 

## Example

```python
from halo_client.models.backup_spec import BackupSpec

# TODO update the JSON string below
json = "{}"
# create an instance of BackupSpec from a JSON string
backup_spec_instance = BackupSpec.from_json(json)
# print the JSON string representation of the object
print(BackupSpec.to_json())

# convert the object into a dict
backup_spec_dict = backup_spec_instance.to_dict()
# create an instance of BackupSpec from a dict
backup_spec_from_dict = BackupSpec.from_dict(backup_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


