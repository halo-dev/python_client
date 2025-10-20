# halo_client.SinglePageV1alpha1ConsoleApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_single_page_content**](SinglePageV1alpha1ConsoleApi.md#delete_single_page_content) | **DELETE** /apis/api.console.halo.run/v1alpha1/singlepages/{name}/content | 
[**draft_single_page**](SinglePageV1alpha1ConsoleApi.md#draft_single_page) | **POST** /apis/api.console.halo.run/v1alpha1/singlepages | 
[**fetch_single_page_content**](SinglePageV1alpha1ConsoleApi.md#fetch_single_page_content) | **GET** /apis/api.console.halo.run/v1alpha1/singlepages/{name}/content | 
[**fetch_single_page_head_content**](SinglePageV1alpha1ConsoleApi.md#fetch_single_page_head_content) | **GET** /apis/api.console.halo.run/v1alpha1/singlepages/{name}/head-content | 
[**fetch_single_page_release_content**](SinglePageV1alpha1ConsoleApi.md#fetch_single_page_release_content) | **GET** /apis/api.console.halo.run/v1alpha1/singlepages/{name}/release-content | 
[**list_single_page_snapshots**](SinglePageV1alpha1ConsoleApi.md#list_single_page_snapshots) | **GET** /apis/api.console.halo.run/v1alpha1/singlepages/{name}/snapshot | 
[**list_single_pages**](SinglePageV1alpha1ConsoleApi.md#list_single_pages) | **GET** /apis/api.console.halo.run/v1alpha1/singlepages | 
[**publish_single_page**](SinglePageV1alpha1ConsoleApi.md#publish_single_page) | **PUT** /apis/api.console.halo.run/v1alpha1/singlepages/{name}/publish | 
[**revert_to_specified_snapshot_for_single_page**](SinglePageV1alpha1ConsoleApi.md#revert_to_specified_snapshot_for_single_page) | **PUT** /apis/api.console.halo.run/v1alpha1/singlepages/{name}/revert-content | 
[**update_draft_single_page**](SinglePageV1alpha1ConsoleApi.md#update_draft_single_page) | **PUT** /apis/api.console.halo.run/v1alpha1/singlepages/{name} | 
[**update_single_page_content**](SinglePageV1alpha1ConsoleApi.md#update_single_page_content) | **PUT** /apis/api.console.halo.run/v1alpha1/singlepages/{name}/content | 


# **delete_single_page_content**
> ContentWrapper delete_single_page_content(name, snapshot_name)

Delete a content for post.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.content_wrapper import ContentWrapper
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
    api_instance = halo_client.SinglePageV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    snapshot_name = 'snapshot_name_example' # str | 

    try:
        api_response = api_instance.delete_single_page_content(name, snapshot_name)
        print("The response of SinglePageV1alpha1ConsoleApi->delete_single_page_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SinglePageV1alpha1ConsoleApi->delete_single_page_content: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **snapshot_name** | **str**|  | 

### Return type

[**ContentWrapper**](ContentWrapper.md)

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

# **draft_single_page**
> SinglePage draft_single_page(single_page_request)

Draft a single page.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.single_page import SinglePage
from halo_client.models.single_page_request import SinglePageRequest
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
    api_instance = halo_client.SinglePageV1alpha1ConsoleApi(api_client)
    single_page_request = halo_client.SinglePageRequest() # SinglePageRequest | 

    try:
        api_response = api_instance.draft_single_page(single_page_request)
        print("The response of SinglePageV1alpha1ConsoleApi->draft_single_page:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SinglePageV1alpha1ConsoleApi->draft_single_page: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **single_page_request** | [**SinglePageRequest**](SinglePageRequest.md)|  | 

### Return type

[**SinglePage**](SinglePage.md)

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

# **fetch_single_page_content**
> ContentWrapper fetch_single_page_content(name, snapshot_name)

Fetch content of single page.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.content_wrapper import ContentWrapper
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
    api_instance = halo_client.SinglePageV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    snapshot_name = 'snapshot_name_example' # str | 

    try:
        api_response = api_instance.fetch_single_page_content(name, snapshot_name)
        print("The response of SinglePageV1alpha1ConsoleApi->fetch_single_page_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SinglePageV1alpha1ConsoleApi->fetch_single_page_content: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **snapshot_name** | **str**|  | 

### Return type

[**ContentWrapper**](ContentWrapper.md)

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

# **fetch_single_page_head_content**
> ContentWrapper fetch_single_page_head_content(name)

Fetch head content of single page.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.content_wrapper import ContentWrapper
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
    api_instance = halo_client.SinglePageV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.fetch_single_page_head_content(name)
        print("The response of SinglePageV1alpha1ConsoleApi->fetch_single_page_head_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SinglePageV1alpha1ConsoleApi->fetch_single_page_head_content: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

[**ContentWrapper**](ContentWrapper.md)

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

# **fetch_single_page_release_content**
> ContentWrapper fetch_single_page_release_content(name)

Fetch release content of single page.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.content_wrapper import ContentWrapper
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
    api_instance = halo_client.SinglePageV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.fetch_single_page_release_content(name)
        print("The response of SinglePageV1alpha1ConsoleApi->fetch_single_page_release_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SinglePageV1alpha1ConsoleApi->fetch_single_page_release_content: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

[**ContentWrapper**](ContentWrapper.md)

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

# **list_single_page_snapshots**
> List[ListedSnapshotDto] list_single_page_snapshots(name)

List all snapshots for single page content.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.listed_snapshot_dto import ListedSnapshotDto
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
    api_instance = halo_client.SinglePageV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.list_single_page_snapshots(name)
        print("The response of SinglePageV1alpha1ConsoleApi->list_single_page_snapshots:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SinglePageV1alpha1ConsoleApi->list_single_page_snapshots: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

[**List[ListedSnapshotDto]**](ListedSnapshotDto.md)

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

# **list_single_pages**
> ListedSinglePageList list_single_pages(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort, contributor=contributor, publish_phase=publish_phase, visible=visible, keyword=keyword)

List single pages.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.listed_single_page_list import ListedSinglePageList
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
    api_instance = halo_client.SinglePageV1alpha1ConsoleApi(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)
    contributor = ['contributor_example'] # List[str] | SinglePages filtered by contributor. (optional)
    publish_phase = 'publish_phase_example' # str | SinglePages filtered by publish phase. (optional)
    visible = 'visible_example' # str | SinglePages filtered by visibility. (optional)
    keyword = 'keyword_example' # str | SinglePages filtered by keyword. (optional)

    try:
        api_response = api_instance.list_single_pages(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort, contributor=contributor, publish_phase=publish_phase, visible=visible, keyword=keyword)
        print("The response of SinglePageV1alpha1ConsoleApi->list_single_pages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SinglePageV1alpha1ConsoleApi->list_single_pages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**| Page number. Default is 0. | [optional] 
 **size** | **int**| Size number. Default is 0. | [optional] 
 **label_selector** | [**List[str]**](str.md)| Label selector. e.g.: hidden!&#x3D;true | [optional] 
 **field_selector** | [**List[str]**](str.md)| Field selector. e.g.: metadata.name&#x3D;&#x3D;halo | [optional] 
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 
 **contributor** | [**List[str]**](str.md)| SinglePages filtered by contributor. | [optional] 
 **publish_phase** | **str**| SinglePages filtered by publish phase. | [optional] 
 **visible** | **str**| SinglePages filtered by visibility. | [optional] 
 **keyword** | **str**| SinglePages filtered by keyword. | [optional] 

### Return type

[**ListedSinglePageList**](ListedSinglePageList.md)

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

# **publish_single_page**
> SinglePage publish_single_page(name)

Publish a single page.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.single_page import SinglePage
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
    api_instance = halo_client.SinglePageV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.publish_single_page(name)
        print("The response of SinglePageV1alpha1ConsoleApi->publish_single_page:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SinglePageV1alpha1ConsoleApi->publish_single_page: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

[**SinglePage**](SinglePage.md)

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

# **revert_to_specified_snapshot_for_single_page**
> Post revert_to_specified_snapshot_for_single_page(name, revert_snapshot_for_single_param)

Revert to specified snapshot for single page content.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.post import Post
from halo_client.models.revert_snapshot_for_single_param import RevertSnapshotForSingleParam
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
    api_instance = halo_client.SinglePageV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    revert_snapshot_for_single_param = halo_client.RevertSnapshotForSingleParam() # RevertSnapshotForSingleParam | 

    try:
        api_response = api_instance.revert_to_specified_snapshot_for_single_page(name, revert_snapshot_for_single_param)
        print("The response of SinglePageV1alpha1ConsoleApi->revert_to_specified_snapshot_for_single_page:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SinglePageV1alpha1ConsoleApi->revert_to_specified_snapshot_for_single_page: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **revert_snapshot_for_single_param** | [**RevertSnapshotForSingleParam**](RevertSnapshotForSingleParam.md)|  | 

### Return type

[**Post**](Post.md)

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

# **update_draft_single_page**
> SinglePage update_draft_single_page(name, single_page_request)

Update a single page.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.single_page import SinglePage
from halo_client.models.single_page_request import SinglePageRequest
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
    api_instance = halo_client.SinglePageV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    single_page_request = halo_client.SinglePageRequest() # SinglePageRequest | 

    try:
        api_response = api_instance.update_draft_single_page(name, single_page_request)
        print("The response of SinglePageV1alpha1ConsoleApi->update_draft_single_page:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SinglePageV1alpha1ConsoleApi->update_draft_single_page: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **single_page_request** | [**SinglePageRequest**](SinglePageRequest.md)|  | 

### Return type

[**SinglePage**](SinglePage.md)

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

# **update_single_page_content**
> Post update_single_page_content(name, content)

Update a single page's content.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.content import Content
from halo_client.models.post import Post
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
    api_instance = halo_client.SinglePageV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    content = halo_client.Content() # Content | 

    try:
        api_response = api_instance.update_single_page_content(name, content)
        print("The response of SinglePageV1alpha1ConsoleApi->update_single_page_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SinglePageV1alpha1ConsoleApi->update_single_page_content: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **content** | [**Content**](Content.md)|  | 

### Return type

[**Post**](Post.md)

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

