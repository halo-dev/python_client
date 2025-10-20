# halo_client.MigrationV1alpha1ConsoleApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**download_backups**](MigrationV1alpha1ConsoleApi.md#download_backups) | **GET** /apis/console.api.migration.halo.run/v1alpha1/backups/{name}/files/{filename} | 
[**get_backup_files**](MigrationV1alpha1ConsoleApi.md#get_backup_files) | **GET** /apis/console.api.migration.halo.run/v1alpha1/backup-files | 
[**restore_backup**](MigrationV1alpha1ConsoleApi.md#restore_backup) | **POST** /apis/console.api.migration.halo.run/v1alpha1/restorations | 


# **download_backups**
> download_backups(name, filename)

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8091
# See configuration.py for a list of all supported configuration parameters.
configuration = halo_client.Configuration(
    host = "http://localhost:8091"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = halo_client.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Configure Bearer authorization (JWT): bearerAuth
configuration = halo_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with halo_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = halo_client.MigrationV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | Backup name.
    filename = 'filename_example' # str | Backup filename.

    try:
        api_instance.download_backups(name, filename)
    except Exception as e:
        print("Exception when calling MigrationV1alpha1ConsoleApi->download_backups: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Backup name. | 
 **filename** | **str**| Backup filename. | 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_backup_files**
> List[BackupFile] get_backup_files()

Get backup files from backup root.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.backup_file import BackupFile
from halo_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8091
# See configuration.py for a list of all supported configuration parameters.
configuration = halo_client.Configuration(
    host = "http://localhost:8091"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = halo_client.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Configure Bearer authorization (JWT): bearerAuth
configuration = halo_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with halo_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = halo_client.MigrationV1alpha1ConsoleApi(api_client)

    try:
        api_response = api_instance.get_backup_files()
        print("The response of MigrationV1alpha1ConsoleApi->get_backup_files:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MigrationV1alpha1ConsoleApi->get_backup_files: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[BackupFile]**](BackupFile.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**0** | default response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **restore_backup**
> restore_backup(backup_name=backup_name, download_url=download_url, file=file, filename=filename)

Restore backup by uploading file or providing download link or backup name.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8091
# See configuration.py for a list of all supported configuration parameters.
configuration = halo_client.Configuration(
    host = "http://localhost:8091"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = halo_client.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Configure Bearer authorization (JWT): bearerAuth
configuration = halo_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with halo_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = halo_client.MigrationV1alpha1ConsoleApi(api_client)
    backup_name = 'backup_name_example' # str | Backup metadata name. (optional)
    download_url = 'download_url_example' # str | Remote backup HTTP URL. (optional)
    file = None # bytearray |  (optional)
    filename = 'filename_example' # str | Filename of backup file in backups root. (optional)

    try:
        api_instance.restore_backup(backup_name=backup_name, download_url=download_url, file=file, filename=filename)
    except Exception as e:
        print("Exception when calling MigrationV1alpha1ConsoleApi->restore_backup: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **backup_name** | **str**| Backup metadata name. | [optional] 
 **download_url** | **str**| Remote backup HTTP URL. | [optional] 
 **file** | **bytearray**|  | [optional] 
 **filename** | **str**| Filename of backup file in backups root. | [optional] 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined


[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

