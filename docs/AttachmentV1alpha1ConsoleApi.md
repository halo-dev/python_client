# halo_client.AttachmentV1alpha1ConsoleApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**external_transfer_attachment**](AttachmentV1alpha1ConsoleApi.md#external_transfer_attachment) | **POST** /apis/api.console.halo.run/v1alpha1/attachments/-/upload-from-url | 
[**search_attachments**](AttachmentV1alpha1ConsoleApi.md#search_attachments) | **GET** /apis/api.console.halo.run/v1alpha1/attachments | 
[**upload_attachment**](AttachmentV1alpha1ConsoleApi.md#upload_attachment) | **POST** /apis/api.console.halo.run/v1alpha1/attachments/upload | 


# **external_transfer_attachment**
> Attachment external_transfer_attachment(upload_from_url_request)

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.attachment import Attachment
from halo_client.models.upload_from_url_request import UploadFromUrlRequest
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
    api_instance = halo_client.AttachmentV1alpha1ConsoleApi(api_client)
    upload_from_url_request = halo_client.UploadFromUrlRequest() # UploadFromUrlRequest | 

    try:
        api_response = api_instance.external_transfer_attachment(upload_from_url_request)
        print("The response of AttachmentV1alpha1ConsoleApi->external_transfer_attachment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AttachmentV1alpha1ConsoleApi->external_transfer_attachment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **upload_from_url_request** | [**UploadFromUrlRequest**](UploadFromUrlRequest.md)|  | 

### Return type

[**Attachment**](Attachment.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**0** | default response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **search_attachments**
> AttachmentList search_attachments(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort, ungrouped=ungrouped, keyword=keyword, accepts=accepts)

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.attachment_list import AttachmentList
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
    api_instance = halo_client.AttachmentV1alpha1ConsoleApi(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)
    ungrouped = True # bool | Filter attachments without group. This parameter will ignore group parameter. (optional)
    keyword = 'keyword_example' # str | Keyword for searching. (optional)
    accepts = ['accepts_example'] # List[str] | Acceptable media types. (optional)

    try:
        api_response = api_instance.search_attachments(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort, ungrouped=ungrouped, keyword=keyword, accepts=accepts)
        print("The response of AttachmentV1alpha1ConsoleApi->search_attachments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AttachmentV1alpha1ConsoleApi->search_attachments: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**| Page number. Default is 0. | [optional] 
 **size** | **int**| Size number. Default is 0. | [optional] 
 **label_selector** | [**List[str]**](str.md)| Label selector. e.g.: hidden!&#x3D;true | [optional] 
 **field_selector** | [**List[str]**](str.md)| Field selector. e.g.: metadata.name&#x3D;&#x3D;halo | [optional] 
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 
 **ungrouped** | **bool**| Filter attachments without group. This parameter will ignore group parameter. | [optional] 
 **keyword** | **str**| Keyword for searching. | [optional] 
 **accepts** | [**List[str]**](str.md)| Acceptable media types. | [optional] 

### Return type

[**AttachmentList**](AttachmentList.md)

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

# **upload_attachment**
> Attachment upload_attachment(file, policy_name, group_name=group_name)

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.attachment import Attachment
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
    api_instance = halo_client.AttachmentV1alpha1ConsoleApi(api_client)
    file = None # bytearray | 
    policy_name = 'policy_name_example' # str | Storage policy name
    group_name = 'group_name_example' # str | The name of the group to which the attachment belongs (optional)

    try:
        api_response = api_instance.upload_attachment(file, policy_name, group_name=group_name)
        print("The response of AttachmentV1alpha1ConsoleApi->upload_attachment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AttachmentV1alpha1ConsoleApi->upload_attachment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | **bytearray**|  | 
 **policy_name** | **str**| Storage policy name | 
 **group_name** | **str**| The name of the group to which the attachment belongs | [optional] 

### Return type

[**Attachment**](Attachment.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**0** | default response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

