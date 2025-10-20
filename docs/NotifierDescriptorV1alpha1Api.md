# halo_client.NotifierDescriptorV1alpha1Api

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_notifier_descriptor**](NotifierDescriptorV1alpha1Api.md#create_notifier_descriptor) | **POST** /apis/notification.halo.run/v1alpha1/notifierDescriptors | 
[**delete_notifier_descriptor**](NotifierDescriptorV1alpha1Api.md#delete_notifier_descriptor) | **DELETE** /apis/notification.halo.run/v1alpha1/notifierDescriptors/{name} | 
[**get_notifier_descriptor**](NotifierDescriptorV1alpha1Api.md#get_notifier_descriptor) | **GET** /apis/notification.halo.run/v1alpha1/notifierDescriptors/{name} | 
[**list_notifier_descriptor**](NotifierDescriptorV1alpha1Api.md#list_notifier_descriptor) | **GET** /apis/notification.halo.run/v1alpha1/notifierDescriptors | 
[**patch_notifier_descriptor**](NotifierDescriptorV1alpha1Api.md#patch_notifier_descriptor) | **PATCH** /apis/notification.halo.run/v1alpha1/notifierDescriptors/{name} | 
[**update_notifier_descriptor**](NotifierDescriptorV1alpha1Api.md#update_notifier_descriptor) | **PUT** /apis/notification.halo.run/v1alpha1/notifierDescriptors/{name} | 


# **create_notifier_descriptor**
> NotifierDescriptor create_notifier_descriptor(notifier_descriptor=notifier_descriptor)

Create NotifierDescriptor

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.notifier_descriptor import NotifierDescriptor
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
    api_instance = halo_client.NotifierDescriptorV1alpha1Api(api_client)
    notifier_descriptor = halo_client.NotifierDescriptor() # NotifierDescriptor | Fresh notifierDescriptor (optional)

    try:
        api_response = api_instance.create_notifier_descriptor(notifier_descriptor=notifier_descriptor)
        print("The response of NotifierDescriptorV1alpha1Api->create_notifier_descriptor:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotifierDescriptorV1alpha1Api->create_notifier_descriptor: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **notifier_descriptor** | [**NotifierDescriptor**](NotifierDescriptor.md)| Fresh notifierDescriptor | [optional] 

### Return type

[**NotifierDescriptor**](NotifierDescriptor.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response notifierDescriptors created just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_notifier_descriptor**
> delete_notifier_descriptor(name)

Delete NotifierDescriptor

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
    api_instance = halo_client.NotifierDescriptorV1alpha1Api(api_client)
    name = 'name_example' # str | Name of notifierDescriptor

    try:
        api_instance.delete_notifier_descriptor(name)
    except Exception as e:
        print("Exception when calling NotifierDescriptorV1alpha1Api->delete_notifier_descriptor: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of notifierDescriptor | 

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
**200** | Response notifierDescriptor deleted just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_notifier_descriptor**
> NotifierDescriptor get_notifier_descriptor(name)

Get NotifierDescriptor

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.notifier_descriptor import NotifierDescriptor
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
    api_instance = halo_client.NotifierDescriptorV1alpha1Api(api_client)
    name = 'name_example' # str | Name of notifierDescriptor

    try:
        api_response = api_instance.get_notifier_descriptor(name)
        print("The response of NotifierDescriptorV1alpha1Api->get_notifier_descriptor:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotifierDescriptorV1alpha1Api->get_notifier_descriptor: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of notifierDescriptor | 

### Return type

[**NotifierDescriptor**](NotifierDescriptor.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response single notifierDescriptor |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_notifier_descriptor**
> NotifierDescriptorList list_notifier_descriptor(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)

List NotifierDescriptor

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.notifier_descriptor_list import NotifierDescriptorList
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
    api_instance = halo_client.NotifierDescriptorV1alpha1Api(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        api_response = api_instance.list_notifier_descriptor(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)
        print("The response of NotifierDescriptorV1alpha1Api->list_notifier_descriptor:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotifierDescriptorV1alpha1Api->list_notifier_descriptor: %s\n" % e)
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

[**NotifierDescriptorList**](NotifierDescriptorList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response notifierDescriptors |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_notifier_descriptor**
> NotifierDescriptor patch_notifier_descriptor(name, json_patch_inner=json_patch_inner)

Patch NotifierDescriptor

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.json_patch_inner import JsonPatchInner
from halo_client.models.notifier_descriptor import NotifierDescriptor
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
    api_instance = halo_client.NotifierDescriptorV1alpha1Api(api_client)
    name = 'name_example' # str | Name of notifierDescriptor
    json_patch_inner = [halo_client.JsonPatchInner()] # List[JsonPatchInner] |  (optional)

    try:
        api_response = api_instance.patch_notifier_descriptor(name, json_patch_inner=json_patch_inner)
        print("The response of NotifierDescriptorV1alpha1Api->patch_notifier_descriptor:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotifierDescriptorV1alpha1Api->patch_notifier_descriptor: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of notifierDescriptor | 
 **json_patch_inner** | [**List[JsonPatchInner]**](JsonPatchInner.md)|  | [optional] 

### Return type

[**NotifierDescriptor**](NotifierDescriptor.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json-patch+json
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response notifierDescriptor patched just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_notifier_descriptor**
> NotifierDescriptor update_notifier_descriptor(name, notifier_descriptor=notifier_descriptor)

Update NotifierDescriptor

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.notifier_descriptor import NotifierDescriptor
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
    api_instance = halo_client.NotifierDescriptorV1alpha1Api(api_client)
    name = 'name_example' # str | Name of notifierDescriptor
    notifier_descriptor = halo_client.NotifierDescriptor() # NotifierDescriptor | Updated notifierDescriptor (optional)

    try:
        api_response = api_instance.update_notifier_descriptor(name, notifier_descriptor=notifier_descriptor)
        print("The response of NotifierDescriptorV1alpha1Api->update_notifier_descriptor:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotifierDescriptorV1alpha1Api->update_notifier_descriptor: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of notifierDescriptor | 
 **notifier_descriptor** | [**NotifierDescriptor**](NotifierDescriptor.md)| Updated notifierDescriptor | [optional] 

### Return type

[**NotifierDescriptor**](NotifierDescriptor.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response notifierDescriptors updated just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

