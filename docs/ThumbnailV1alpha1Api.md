# halo_client.ThumbnailV1alpha1Api

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_thumbnail**](ThumbnailV1alpha1Api.md#create_thumbnail) | **POST** /apis/storage.halo.run/v1alpha1/thumbnails | 
[**delete_thumbnail**](ThumbnailV1alpha1Api.md#delete_thumbnail) | **DELETE** /apis/storage.halo.run/v1alpha1/thumbnails/{name} | 
[**get_thumbnail**](ThumbnailV1alpha1Api.md#get_thumbnail) | **GET** /apis/storage.halo.run/v1alpha1/thumbnails/{name} | 
[**list_thumbnail**](ThumbnailV1alpha1Api.md#list_thumbnail) | **GET** /apis/storage.halo.run/v1alpha1/thumbnails | 
[**patch_thumbnail**](ThumbnailV1alpha1Api.md#patch_thumbnail) | **PATCH** /apis/storage.halo.run/v1alpha1/thumbnails/{name} | 
[**update_thumbnail**](ThumbnailV1alpha1Api.md#update_thumbnail) | **PUT** /apis/storage.halo.run/v1alpha1/thumbnails/{name} | 


# **create_thumbnail**
> Thumbnail create_thumbnail(thumbnail=thumbnail)

Create Thumbnail

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.thumbnail import Thumbnail
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
    api_instance = halo_client.ThumbnailV1alpha1Api(api_client)
    thumbnail = halo_client.Thumbnail() # Thumbnail | Fresh thumbnail (optional)

    try:
        api_response = api_instance.create_thumbnail(thumbnail=thumbnail)
        print("The response of ThumbnailV1alpha1Api->create_thumbnail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ThumbnailV1alpha1Api->create_thumbnail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **thumbnail** | [**Thumbnail**](Thumbnail.md)| Fresh thumbnail | [optional] 

### Return type

[**Thumbnail**](Thumbnail.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response thumbnails created just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_thumbnail**
> delete_thumbnail(name)

Delete Thumbnail

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
    api_instance = halo_client.ThumbnailV1alpha1Api(api_client)
    name = 'name_example' # str | Name of thumbnail

    try:
        api_instance.delete_thumbnail(name)
    except Exception as e:
        print("Exception when calling ThumbnailV1alpha1Api->delete_thumbnail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of thumbnail | 

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
**200** | Response thumbnail deleted just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_thumbnail**
> Thumbnail get_thumbnail(name)

Get Thumbnail

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.thumbnail import Thumbnail
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
    api_instance = halo_client.ThumbnailV1alpha1Api(api_client)
    name = 'name_example' # str | Name of thumbnail

    try:
        api_response = api_instance.get_thumbnail(name)
        print("The response of ThumbnailV1alpha1Api->get_thumbnail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ThumbnailV1alpha1Api->get_thumbnail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of thumbnail | 

### Return type

[**Thumbnail**](Thumbnail.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response single thumbnail |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_thumbnail**
> ThumbnailList list_thumbnail(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)

List Thumbnail

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.thumbnail_list import ThumbnailList
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
    api_instance = halo_client.ThumbnailV1alpha1Api(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        api_response = api_instance.list_thumbnail(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)
        print("The response of ThumbnailV1alpha1Api->list_thumbnail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ThumbnailV1alpha1Api->list_thumbnail: %s\n" % e)
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

[**ThumbnailList**](ThumbnailList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response thumbnails |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_thumbnail**
> Thumbnail patch_thumbnail(name, json_patch_inner=json_patch_inner)

Patch Thumbnail

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.json_patch_inner import JsonPatchInner
from halo_client.models.thumbnail import Thumbnail
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
    api_instance = halo_client.ThumbnailV1alpha1Api(api_client)
    name = 'name_example' # str | Name of thumbnail
    json_patch_inner = [halo_client.JsonPatchInner()] # List[JsonPatchInner] |  (optional)

    try:
        api_response = api_instance.patch_thumbnail(name, json_patch_inner=json_patch_inner)
        print("The response of ThumbnailV1alpha1Api->patch_thumbnail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ThumbnailV1alpha1Api->patch_thumbnail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of thumbnail | 
 **json_patch_inner** | [**List[JsonPatchInner]**](JsonPatchInner.md)|  | [optional] 

### Return type

[**Thumbnail**](Thumbnail.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json-patch+json
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response thumbnail patched just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_thumbnail**
> Thumbnail update_thumbnail(name, thumbnail=thumbnail)

Update Thumbnail

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.thumbnail import Thumbnail
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
    api_instance = halo_client.ThumbnailV1alpha1Api(api_client)
    name = 'name_example' # str | Name of thumbnail
    thumbnail = halo_client.Thumbnail() # Thumbnail | Updated thumbnail (optional)

    try:
        api_response = api_instance.update_thumbnail(name, thumbnail=thumbnail)
        print("The response of ThumbnailV1alpha1Api->update_thumbnail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ThumbnailV1alpha1Api->update_thumbnail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of thumbnail | 
 **thumbnail** | [**Thumbnail**](Thumbnail.md)| Updated thumbnail | [optional] 

### Return type

[**Thumbnail**](Thumbnail.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response thumbnails updated just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

