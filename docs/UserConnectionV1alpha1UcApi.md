# halo_client.UserConnectionV1alpha1UcApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**disconnect_my_connection**](UserConnectionV1alpha1UcApi.md#disconnect_my_connection) | **PUT** /apis/uc.api.auth.halo.run/v1alpha1/user-connections/{registerId}/disconnect | 


# **disconnect_my_connection**
> List[UserConnection] disconnect_my_connection(register_id)

Disconnect my connection from a third-party platform.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.user_connection import UserConnection
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
    api_instance = halo_client.UserConnectionV1alpha1UcApi(api_client)
    register_id = 'register_id_example' # str | The registration ID of the third-party platform.

    try:
        api_response = api_instance.disconnect_my_connection(register_id)
        print("The response of UserConnectionV1alpha1UcApi->disconnect_my_connection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserConnectionV1alpha1UcApi->disconnect_my_connection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **register_id** | **str**| The registration ID of the third-party platform. | 

### Return type

[**List[UserConnection]**](UserConnection.md)

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

