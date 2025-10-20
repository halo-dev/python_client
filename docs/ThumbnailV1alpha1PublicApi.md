# halo_client.ThumbnailV1alpha1PublicApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_thumbnail_by_uri**](ThumbnailV1alpha1PublicApi.md#get_thumbnail_by_uri) | **GET** /apis/api.storage.halo.run/v1alpha1/thumbnails/-/via-uri | 


# **get_thumbnail_by_uri**
> bytearray get_thumbnail_by_uri(uri, size)

Get thumbnail by URI

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
    api_instance = halo_client.ThumbnailV1alpha1PublicApi(api_client)
    uri = 'uri_example' # str | The URI of the image
    size = 'size_example' # str | The size of the thumbnail,available values are s,m,l,xl

    try:
        api_response = api_instance.get_thumbnail_by_uri(uri, size)
        print("The response of ThumbnailV1alpha1PublicApi->get_thumbnail_by_uri:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ThumbnailV1alpha1PublicApi->get_thumbnail_by_uri: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uri** | **str**| The URI of the image | 
 **size** | **str**| The size of the thumbnail,available values are s,m,l,xl | 

### Return type

**bytearray**

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

