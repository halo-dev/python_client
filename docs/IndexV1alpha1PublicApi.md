# halo_client.IndexV1alpha1PublicApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**indices_search**](IndexV1alpha1PublicApi.md#indices_search) | **POST** /apis/api.halo.run/v1alpha1/indices/-/search | 


# **indices_search**
> SearchResult indices_search(search_option=search_option)

Search indices.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.search_option import SearchOption
from halo_client.models.search_result import SearchResult
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
    api_instance = halo_client.IndexV1alpha1PublicApi(api_client)
    search_option = halo_client.SearchOption() # SearchOption | Please note that the \"filterPublished\", \"filterExposed\" and \"filterRecycled\" fields are ignored in this endpoint. (optional)

    try:
        api_response = api_instance.indices_search(search_option=search_option)
        print("The response of IndexV1alpha1PublicApi->indices_search:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IndexV1alpha1PublicApi->indices_search: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search_option** | [**SearchOption**](SearchOption.md)| Please note that the \&quot;filterPublished\&quot;, \&quot;filterExposed\&quot; and \&quot;filterRecycled\&quot; fields are ignored in this endpoint. | [optional] 

### Return type

[**SearchResult**](SearchResult.md)

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

