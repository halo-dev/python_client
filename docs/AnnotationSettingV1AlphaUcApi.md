# halo_client.AnnotationSettingV1AlphaUcApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_available_annotation_settings**](AnnotationSettingV1AlphaUcApi.md#list_available_annotation_settings) | **GET** /apis/uc.api.halo.run/v1alpha1/annotationsettings | 


# **list_available_annotation_settings**
> List[AnnotationSetting] list_available_annotation_settings(target_ref)

List available AnnotationSettings for the given targetRef. The available AnnotationSettings are determined by the currently activated theme and started plugins.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.annotation_setting import AnnotationSetting
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
    api_instance = halo_client.AnnotationSettingV1AlphaUcApi(api_client)
    target_ref = 'target_ref_example' # str | The targetRef of the AnnotationSetting. e.g.: 'content.halo.run/Post

    try:
        api_response = api_instance.list_available_annotation_settings(target_ref)
        print("The response of AnnotationSettingV1AlphaUcApi->list_available_annotation_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnnotationSettingV1AlphaUcApi->list_available_annotation_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **target_ref** | **str**| The targetRef of the AnnotationSetting. e.g.: &#39;content.halo.run/Post | 

### Return type

[**List[AnnotationSetting]**](AnnotationSetting.md)

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

