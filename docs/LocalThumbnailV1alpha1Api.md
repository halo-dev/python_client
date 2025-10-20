# halo_client.LocalThumbnailV1alpha1Api

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_local_thumbnail**](LocalThumbnailV1alpha1Api.md#create_local_thumbnail) | **POST** /apis/storage.halo.run/v1alpha1/localthumbnails | 
[**delete_local_thumbnail**](LocalThumbnailV1alpha1Api.md#delete_local_thumbnail) | **DELETE** /apis/storage.halo.run/v1alpha1/localthumbnails/{name} | 
[**get_local_thumbnail**](LocalThumbnailV1alpha1Api.md#get_local_thumbnail) | **GET** /apis/storage.halo.run/v1alpha1/localthumbnails/{name} | 
[**list_local_thumbnail**](LocalThumbnailV1alpha1Api.md#list_local_thumbnail) | **GET** /apis/storage.halo.run/v1alpha1/localthumbnails | 
[**patch_local_thumbnail**](LocalThumbnailV1alpha1Api.md#patch_local_thumbnail) | **PATCH** /apis/storage.halo.run/v1alpha1/localthumbnails/{name} | 
[**update_local_thumbnail**](LocalThumbnailV1alpha1Api.md#update_local_thumbnail) | **PUT** /apis/storage.halo.run/v1alpha1/localthumbnails/{name} | 


# **create_local_thumbnail**
> LocalThumbnail create_local_thumbnail(local_thumbnail=local_thumbnail)

Create LocalThumbnail

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.local_thumbnail import LocalThumbnail
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
    api_instance = halo_client.LocalThumbnailV1alpha1Api(api_client)
    local_thumbnail = halo_client.LocalThumbnail() # LocalThumbnail | Fresh localthumbnail (optional)

    try:
        api_response = api_instance.create_local_thumbnail(local_thumbnail=local_thumbnail)
        print("The response of LocalThumbnailV1alpha1Api->create_local_thumbnail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocalThumbnailV1alpha1Api->create_local_thumbnail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **local_thumbnail** | [**LocalThumbnail**](LocalThumbnail.md)| Fresh localthumbnail | [optional] 

### Return type

[**LocalThumbnail**](LocalThumbnail.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response localthumbnails created just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_local_thumbnail**
> delete_local_thumbnail(name)

Delete LocalThumbnail

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
    api_instance = halo_client.LocalThumbnailV1alpha1Api(api_client)
    name = 'name_example' # str | Name of localthumbnail

    try:
        api_instance.delete_local_thumbnail(name)
    except Exception as e:
        print("Exception when calling LocalThumbnailV1alpha1Api->delete_local_thumbnail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of localthumbnail | 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response localthumbnail deleted just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_local_thumbnail**
> LocalThumbnail get_local_thumbnail(name)

Get LocalThumbnail

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.local_thumbnail import LocalThumbnail
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
    api_instance = halo_client.LocalThumbnailV1alpha1Api(api_client)
    name = 'name_example' # str | Name of localthumbnail

    try:
        api_response = api_instance.get_local_thumbnail(name)
        print("The response of LocalThumbnailV1alpha1Api->get_local_thumbnail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocalThumbnailV1alpha1Api->get_local_thumbnail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of localthumbnail | 

### Return type

[**LocalThumbnail**](LocalThumbnail.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response single localthumbnail |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_local_thumbnail**
> LocalThumbnailList list_local_thumbnail(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)

List LocalThumbnail

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.local_thumbnail_list import LocalThumbnailList
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
    api_instance = halo_client.LocalThumbnailV1alpha1Api(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        api_response = api_instance.list_local_thumbnail(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)
        print("The response of LocalThumbnailV1alpha1Api->list_local_thumbnail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocalThumbnailV1alpha1Api->list_local_thumbnail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**| Page number. Default is 0. | [optional] 
 **size** | **int**| Size number. Default is 0. | [optional] 
 **label_selector** | [**List[str]**](str.md)| Label selector. e.g.: hidden!&#x3D;true | [optional] 
 **field_selector** | [**List[str]**](str.md)| Field selector. e.g.: metadata.name&#x3D;&#x3D;halo | [optional] 
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 

### Return type

[**LocalThumbnailList**](LocalThumbnailList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response localthumbnails |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_local_thumbnail**
> LocalThumbnail patch_local_thumbnail(name, json_patch_inner=json_patch_inner)

Patch LocalThumbnail

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.json_patch_inner import JsonPatchInner
from halo_client.models.local_thumbnail import LocalThumbnail
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
    api_instance = halo_client.LocalThumbnailV1alpha1Api(api_client)
    name = 'name_example' # str | Name of localthumbnail
    json_patch_inner = [halo_client.JsonPatchInner()] # List[JsonPatchInner] |  (optional)

    try:
        api_response = api_instance.patch_local_thumbnail(name, json_patch_inner=json_patch_inner)
        print("The response of LocalThumbnailV1alpha1Api->patch_local_thumbnail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocalThumbnailV1alpha1Api->patch_local_thumbnail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of localthumbnail | 
 **json_patch_inner** | [**List[JsonPatchInner]**](JsonPatchInner.md)|  | [optional] 

### Return type

[**LocalThumbnail**](LocalThumbnail.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json-patch+json
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response localthumbnail patched just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_local_thumbnail**
> LocalThumbnail update_local_thumbnail(name, local_thumbnail=local_thumbnail)

Update LocalThumbnail

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.local_thumbnail import LocalThumbnail
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
    api_instance = halo_client.LocalThumbnailV1alpha1Api(api_client)
    name = 'name_example' # str | Name of localthumbnail
    local_thumbnail = halo_client.LocalThumbnail() # LocalThumbnail | Updated localthumbnail (optional)

    try:
        api_response = api_instance.update_local_thumbnail(name, local_thumbnail=local_thumbnail)
        print("The response of LocalThumbnailV1alpha1Api->update_local_thumbnail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LocalThumbnailV1alpha1Api->update_local_thumbnail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of localthumbnail | 
 **local_thumbnail** | [**LocalThumbnail**](LocalThumbnail.md)| Updated localthumbnail | [optional] 

### Return type

[**LocalThumbnail**](LocalThumbnail.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response localthumbnails updated just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

