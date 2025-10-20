# halo_client.PolicyAlpha1ConsoleApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_policy_config_by_group**](PolicyAlpha1ConsoleApi.md#get_policy_config_by_group) | **GET** /apis/console.api.storage.halo.run/v1alpha1/policies/{name}/configs/{group} | 
[**update_policy_config_by_group**](PolicyAlpha1ConsoleApi.md#update_policy_config_by_group) | **PUT** /apis/console.api.storage.halo.run/v1alpha1/policies/{name}/configs/{group} | 


# **get_policy_config_by_group**
> object get_policy_config_by_group(name, group)

Get policy config by group

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
    api_instance = halo_client.PolicyAlpha1ConsoleApi(api_client)
    name = 'name_example' # str | Name of the policy
    group = 'group_example' # str | Name of the group

    try:
        api_response = api_instance.get_policy_config_by_group(name, group)
        print("The response of PolicyAlpha1ConsoleApi->get_policy_config_by_group:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PolicyAlpha1ConsoleApi->get_policy_config_by_group: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of the policy | 
 **group** | **str**| Name of the group | 

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

# **update_policy_config_by_group**
> update_policy_config_by_group(name, group, body)

Update policy config by group

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
    api_instance = halo_client.PolicyAlpha1ConsoleApi(api_client)
    name = 'name_example' # str | Name of the policy
    group = 'group_example' # str | Name of the group
    body = None # object | 

    try:
        api_instance.update_policy_config_by_group(name, group, body)
    except Exception as e:
        print("Exception when calling PolicyAlpha1ConsoleApi->update_policy_config_by_group: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of the policy | 
 **group** | **str**| Name of the group | 
 **body** | **object**|  | 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | No Content |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

