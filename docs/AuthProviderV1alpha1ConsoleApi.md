# halo_client.AuthProviderV1alpha1ConsoleApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**disable_auth_provider**](AuthProviderV1alpha1ConsoleApi.md#disable_auth_provider) | **PUT** /apis/api.console.halo.run/v1alpha1/auth-providers/{name}/disable | 
[**enable_auth_provider**](AuthProviderV1alpha1ConsoleApi.md#enable_auth_provider) | **PUT** /apis/api.console.halo.run/v1alpha1/auth-providers/{name}/enable | 
[**list_auth_providers**](AuthProviderV1alpha1ConsoleApi.md#list_auth_providers) | **GET** /apis/api.console.halo.run/v1alpha1/auth-providers | 


# **disable_auth_provider**
> AuthProvider disable_auth_provider(name)

Disables an auth provider

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.auth_provider import AuthProvider
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
    api_instance = halo_client.AuthProviderV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.disable_auth_provider(name)
        print("The response of AuthProviderV1alpha1ConsoleApi->disable_auth_provider:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthProviderV1alpha1ConsoleApi->disable_auth_provider: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

[**AuthProvider**](AuthProvider.md)

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

# **enable_auth_provider**
> AuthProvider enable_auth_provider(name)

Enables an auth provider

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.auth_provider import AuthProvider
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
    api_instance = halo_client.AuthProviderV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.enable_auth_provider(name)
        print("The response of AuthProviderV1alpha1ConsoleApi->enable_auth_provider:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthProviderV1alpha1ConsoleApi->enable_auth_provider: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

[**AuthProvider**](AuthProvider.md)

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

# **list_auth_providers**
> List[ListedAuthProvider] list_auth_providers()

Lists all auth providers

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.listed_auth_provider import ListedAuthProvider
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
    api_instance = halo_client.AuthProviderV1alpha1ConsoleApi(api_client)

    try:
        api_response = api_instance.list_auth_providers()
        print("The response of AuthProviderV1alpha1ConsoleApi->list_auth_providers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthProviderV1alpha1ConsoleApi->list_auth_providers: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[ListedAuthProvider]**](ListedAuthProvider.md)

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

