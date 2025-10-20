# halo_client.NotificationV1alpha1PublicApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**unsubscribe**](NotificationV1alpha1PublicApi.md#unsubscribe) | **GET** /apis/api.notification.halo.run/v1alpha1/subscriptions/{name}/unsubscribe | 


# **unsubscribe**
> str unsubscribe(name, token)

Unsubscribe a subscription

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
    api_instance = halo_client.NotificationV1alpha1PublicApi(api_client)
    name = 'name_example' # str | Subscription name
    token = 'token_example' # str | Unsubscribe token

    try:
        api_response = api_instance.unsubscribe(name, token)
        print("The response of NotificationV1alpha1PublicApi->unsubscribe:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationV1alpha1PublicApi->unsubscribe: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Subscription name | 
 **token** | **str**| Unsubscribe token | 

### Return type

**str**

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

