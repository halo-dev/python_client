# halo_client.AttachmentV1alpha1UcApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_attachment_for_post**](AttachmentV1alpha1UcApi.md#create_attachment_for_post) | **POST** /apis/uc.api.storage.halo.run/v1alpha1/attachments | 
[**external_transfer_attachment1**](AttachmentV1alpha1UcApi.md#external_transfer_attachment1) | **POST** /apis/uc.api.storage.halo.run/v1alpha1/attachments/-/upload-from-url | 
[**list_my_attachments**](AttachmentV1alpha1UcApi.md#list_my_attachments) | **GET** /apis/uc.api.storage.halo.run/v1alpha1/attachments | 
[**upload_attachment_for_uc**](AttachmentV1alpha1UcApi.md#upload_attachment_for_uc) | **POST** /apis/uc.api.storage.halo.run/v1alpha1/attachments/-/upload | 


# **create_attachment_for_post**
> Attachment create_attachment_for_post(file, wait_for_permalink=wait_for_permalink, post_name=post_name, single_page_name=single_page_name)

Create attachment for the given post. Deprecated in favor of /attachments/-/upload.

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
    api_instance = halo_client.AttachmentV1alpha1UcApi(api_client)
    file = None # bytearray | 
    wait_for_permalink = True # bool | Wait for permalink. (optional)
    post_name = 'post_name_example' # str | Post name. (optional)
    single_page_name = 'single_page_name_example' # str | Single page name. (optional)

    try:
        api_response = api_instance.create_attachment_for_post(file, wait_for_permalink=wait_for_permalink, post_name=post_name, single_page_name=single_page_name)
        print("The response of AttachmentV1alpha1UcApi->create_attachment_for_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AttachmentV1alpha1UcApi->create_attachment_for_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | **bytearray**|  | 
 **wait_for_permalink** | **bool**| Wait for permalink. | [optional] 
 **post_name** | **str**| Post name. | [optional] 
 **single_page_name** | **str**| Single page name. | [optional] 

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

# **external_transfer_attachment1**
> Attachment external_transfer_attachment1(uc_upload_from_url_request, wait_for_permalink=wait_for_permalink)

Upload attachment from the given URL.
Deprecated in favor of /attachments/-/upload.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.attachment import Attachment
from halo_client.models.uc_upload_from_url_request import UcUploadFromUrlRequest
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
    api_instance = halo_client.AttachmentV1alpha1UcApi(api_client)
    uc_upload_from_url_request = halo_client.UcUploadFromUrlRequest() # UcUploadFromUrlRequest | 
    wait_for_permalink = True # bool | Wait for permalink. (optional)

    try:
        api_response = api_instance.external_transfer_attachment1(uc_upload_from_url_request, wait_for_permalink=wait_for_permalink)
        print("The response of AttachmentV1alpha1UcApi->external_transfer_attachment1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AttachmentV1alpha1UcApi->external_transfer_attachment1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uc_upload_from_url_request** | [**UcUploadFromUrlRequest**](UcUploadFromUrlRequest.md)|  | 
 **wait_for_permalink** | **bool**| Wait for permalink. | [optional] 

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

# **list_my_attachments**
> AttachmentList list_my_attachments(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort, ungrouped=ungrouped, keyword=keyword, accepts=accepts)

List attachments of the current user uploaded.

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
    api_instance = halo_client.AttachmentV1alpha1UcApi(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)
    ungrouped = True # bool | Filter attachments without group. This parameter will ignore group parameter. (optional)
    keyword = 'keyword_example' # str | Keyword for searching. (optional)
    accepts = ['accepts_example'] # List[str] | Acceptable media types. (optional)

    try:
        api_response = api_instance.list_my_attachments(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort, ungrouped=ungrouped, keyword=keyword, accepts=accepts)
        print("The response of AttachmentV1alpha1UcApi->list_my_attachments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AttachmentV1alpha1UcApi->list_my_attachments: %s\n" % e)
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

# **upload_attachment_for_uc**
> Attachment upload_attachment_for_uc(file=file, filename=filename, url=url)

Upload attachment to user center storage.

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
    api_instance = halo_client.AttachmentV1alpha1UcApi(api_client)
    file = None # bytearray | The file to upload. If not provided, the url will be used. (optional)
    filename = 'filename_example' # str | The filename to use when uploading from url. If not provided, the filename will be  extracted from the url. (optional)
    url = 'url_example' # str | The url to upload from. If not provided, the file will be used. (optional)

    try:
        api_response = api_instance.upload_attachment_for_uc(file=file, filename=filename, url=url)
        print("The response of AttachmentV1alpha1UcApi->upload_attachment_for_uc:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AttachmentV1alpha1UcApi->upload_attachment_for_uc: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | **bytearray**| The file to upload. If not provided, the url will be used. | [optional] 
 **filename** | **str**| The filename to use when uploading from url. If not provided, the filename will be  extracted from the url. | [optional] 
 **url** | **str**| The url to upload from. If not provided, the file will be used. | [optional] 

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

