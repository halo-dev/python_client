# BackupStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**completion_timestamp** | **datetime** |  | [optional] 
**failure_message** | **str** |  | [optional] 
**failure_reason** | **str** |  | [optional] 
**filename** | **str** | Name of backup file. | [optional] 
**phase** | **str** |  | [optional] 
**size** | **int** | Size of backup file. Data unit: byte | [optional] 
**start_timestamp** | **datetime** |  | [optional] 

## Example

```python
from halo_client.models.backup_status import BackupStatus

# TODO update the JSON string below
json = "{}"
# create an instance of BackupStatus from a JSON string
backup_status_instance = BackupStatus.from_json(json)
# print the JSON string representation of the object
print(BackupStatus.to_json())

# convert the object into a dict
backup_status_dict = backup_status_instance.to_dict()
# create an instance of BackupStatus from a dict
backup_status_from_dict = BackupStatus.from_dict(backup_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


