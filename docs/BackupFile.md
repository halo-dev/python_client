# BackupFile

Backup file.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**filename** | **str** | Filename of backup file. | [optional] 
**last_modified_time** | **datetime** | Last modified time of backup file. | [optional] 
**size** | **int** | Size of backup file. | [optional] 

## Example

```python
from halo_client.models.backup_file import BackupFile

# TODO update the JSON string below
json = "{}"
# create an instance of BackupFile from a JSON string
backup_file_instance = BackupFile.from_json(json)
# print the JSON string representation of the object
print(BackupFile.to_json())

# convert the object into a dict
backup_file_dict = backup_file_instance.to_dict()
# create an instance of BackupFile from a dict
backup_file_from_dict = BackupFile.from_dict(backup_file_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


