# halo_client.ReverseProxyV1alpha1Api

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_reverse_proxy**](ReverseProxyV1alpha1Api.md#create_reverse_proxy) | **POST** /apis/plugin.halo.run/v1alpha1/reverseproxies | 
[**delete_reverse_proxy**](ReverseProxyV1alpha1Api.md#delete_reverse_proxy) | **DELETE** /apis/plugin.halo.run/v1alpha1/reverseproxies/{name} | 
[**get_reverse_proxy**](ReverseProxyV1alpha1Api.md#get_reverse_proxy) | **GET** /apis/plugin.halo.run/v1alpha1/reverseproxies/{name} | 
[**list_reverse_proxy**](ReverseProxyV1alpha1Api.md#list_reverse_proxy) | **GET** /apis/plugin.halo.run/v1alpha1/reverseproxies | 
[**patch_reverse_proxy**](ReverseProxyV1alpha1Api.md#patch_reverse_proxy) | **PATCH** /apis/plugin.halo.run/v1alpha1/reverseproxies/{name} | 
[**update_reverse_proxy**](ReverseProxyV1alpha1Api.md#update_reverse_proxy) | **PUT** /apis/plugin.halo.run/v1alpha1/reverseproxies/{name} | 


# **create_reverse_proxy**
> ReverseProxy create_reverse_proxy(reverse_proxy=reverse_proxy)

Create ReverseProxy

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.reverse_proxy import ReverseProxy
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
    api_instance = halo_client.ReverseProxyV1alpha1Api(api_client)
    reverse_proxy = halo_client.ReverseProxy() # ReverseProxy | Fresh reverseproxy (optional)

    try:
        api_response = api_instance.create_reverse_proxy(reverse_proxy=reverse_proxy)
        print("The response of ReverseProxyV1alpha1Api->create_reverse_proxy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReverseProxyV1alpha1Api->create_reverse_proxy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **reverse_proxy** | [**ReverseProxy**](ReverseProxy.md)| Fresh reverseproxy | [optional] 

### Return type

[**ReverseProxy**](ReverseProxy.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response reverseproxies created just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_reverse_proxy**
> delete_reverse_proxy(name)

Delete ReverseProxy

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
    api_instance = halo_client.ReverseProxyV1alpha1Api(api_client)
    name = 'name_example' # str | Name of reverseproxy

    try:
        api_instance.delete_reverse_proxy(name)
    except Exception as e:
        print("Exception when calling ReverseProxyV1alpha1Api->delete_reverse_proxy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of reverseproxy | 

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
**200** | Response reverseproxy deleted just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_reverse_proxy**
> ReverseProxy get_reverse_proxy(name)

Get ReverseProxy

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.reverse_proxy import ReverseProxy
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
    api_instance = halo_client.ReverseProxyV1alpha1Api(api_client)
    name = 'name_example' # str | Name of reverseproxy

    try:
        api_response = api_instance.get_reverse_proxy(name)
        print("The response of ReverseProxyV1alpha1Api->get_reverse_proxy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReverseProxyV1alpha1Api->get_reverse_proxy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of reverseproxy | 

### Return type

[**ReverseProxy**](ReverseProxy.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response single reverseproxy |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_reverse_proxy**
> ReverseProxyList list_reverse_proxy(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)

List ReverseProxy

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.reverse_proxy_list import ReverseProxyList
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
    api_instance = halo_client.ReverseProxyV1alpha1Api(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        api_response = api_instance.list_reverse_proxy(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)
        print("The response of ReverseProxyV1alpha1Api->list_reverse_proxy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReverseProxyV1alpha1Api->list_reverse_proxy: %s\n" % e)
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

[**ReverseProxyList**](ReverseProxyList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response reverseproxies |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_reverse_proxy**
> ReverseProxy patch_reverse_proxy(name, json_patch_inner=json_patch_inner)

Patch ReverseProxy

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.json_patch_inner import JsonPatchInner
from halo_client.models.reverse_proxy import ReverseProxy
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
    api_instance = halo_client.ReverseProxyV1alpha1Api(api_client)
    name = 'name_example' # str | Name of reverseproxy
    json_patch_inner = [halo_client.JsonPatchInner()] # List[JsonPatchInner] |  (optional)

    try:
        api_response = api_instance.patch_reverse_proxy(name, json_patch_inner=json_patch_inner)
        print("The response of ReverseProxyV1alpha1Api->patch_reverse_proxy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReverseProxyV1alpha1Api->patch_reverse_proxy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of reverseproxy | 
 **json_patch_inner** | [**List[JsonPatchInner]**](JsonPatchInner.md)|  | [optional] 

### Return type

[**ReverseProxy**](ReverseProxy.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json-patch+json
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response reverseproxy patched just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_reverse_proxy**
> ReverseProxy update_reverse_proxy(name, reverse_proxy=reverse_proxy)

Update ReverseProxy

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.reverse_proxy import ReverseProxy
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
    api_instance = halo_client.ReverseProxyV1alpha1Api(api_client)
    name = 'name_example' # str | Name of reverseproxy
    reverse_proxy = halo_client.ReverseProxy() # ReverseProxy | Updated reverseproxy (optional)

    try:
        api_response = api_instance.update_reverse_proxy(name, reverse_proxy=reverse_proxy)
        print("The response of ReverseProxyV1alpha1Api->update_reverse_proxy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReverseProxyV1alpha1Api->update_reverse_proxy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of reverseproxy | 
 **reverse_proxy** | [**ReverseProxy**](ReverseProxy.md)| Updated reverseproxy | [optional] 

### Return type

[**ReverseProxy**](ReverseProxy.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response reverseproxies updated just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

