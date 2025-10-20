# halo_client.UserPreferenceV1alpha1UcApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_my_preference**](UserPreferenceV1alpha1UcApi.md#get_my_preference) | **GET** /apis/uc.api.halo.run/v1alpha1/user-preferences/{group} | 
[**update_my_preference**](UserPreferenceV1alpha1UcApi.md#update_my_preference) | **PUT** /apis/uc.api.halo.run/v1alpha1/user-preferences/{group} | 


# **get_my_preference**
> object get_my_preference(group)

Get my preference by group.

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
    api_instance = halo_client.UserPreferenceV1alpha1UcApi(api_client)
    group = 'group_example' # str | Group of user preference, e.g. `notification`.

    try:
        api_response = api_instance.get_my_preference(group)
        print("The response of UserPreferenceV1alpha1UcApi->get_my_preference:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserPreferenceV1alpha1UcApi->get_my_preference: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group** | **str**| Group of user preference, e.g. &#x60;notification&#x60;. | 

### Return type

**object**

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

# **update_my_preference**
> update_my_preference(group, body)

Create or update my preference by group.

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
    api_instance = halo_client.UserPreferenceV1alpha1UcApi(api_client)
    group = 'group_example' # str | Group of user preference, e.g. `notification`.
    body = None # object | 

    try:
        api_instance.update_my_preference(group, body)
    except Exception as e:
        print("Exception when calling UserPreferenceV1alpha1UcApi->update_my_preference: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group** | **str**| Group of user preference, e.g. &#x60;notification&#x60;. | 
 **body** | **object**|  | 

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
**204** | No content, preference updated successfully. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

