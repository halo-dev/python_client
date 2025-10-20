# halo_client.PostV1alpha1ConsoleApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_post_content**](PostV1alpha1ConsoleApi.md#delete_post_content) | **DELETE** /apis/api.console.halo.run/v1alpha1/posts/{name}/content | 
[**draft_post**](PostV1alpha1ConsoleApi.md#draft_post) | **POST** /apis/api.console.halo.run/v1alpha1/posts | 
[**fetch_post_content**](PostV1alpha1ConsoleApi.md#fetch_post_content) | **GET** /apis/api.console.halo.run/v1alpha1/posts/{name}/content | 
[**fetch_post_head_content**](PostV1alpha1ConsoleApi.md#fetch_post_head_content) | **GET** /apis/api.console.halo.run/v1alpha1/posts/{name}/head-content | 
[**fetch_post_release_content**](PostV1alpha1ConsoleApi.md#fetch_post_release_content) | **GET** /apis/api.console.halo.run/v1alpha1/posts/{name}/release-content | 
[**list_post_snapshots**](PostV1alpha1ConsoleApi.md#list_post_snapshots) | **GET** /apis/api.console.halo.run/v1alpha1/posts/{name}/snapshot | 
[**list_posts**](PostV1alpha1ConsoleApi.md#list_posts) | **GET** /apis/api.console.halo.run/v1alpha1/posts | 
[**publish_post**](PostV1alpha1ConsoleApi.md#publish_post) | **PUT** /apis/api.console.halo.run/v1alpha1/posts/{name}/publish | 
[**recycle_post**](PostV1alpha1ConsoleApi.md#recycle_post) | **PUT** /apis/api.console.halo.run/v1alpha1/posts/{name}/recycle | 
[**revert_to_specified_snapshot_for_post**](PostV1alpha1ConsoleApi.md#revert_to_specified_snapshot_for_post) | **PUT** /apis/api.console.halo.run/v1alpha1/posts/{name}/revert-content | 
[**unpublish_post**](PostV1alpha1ConsoleApi.md#unpublish_post) | **PUT** /apis/api.console.halo.run/v1alpha1/posts/{name}/unpublish | 
[**update_draft_post**](PostV1alpha1ConsoleApi.md#update_draft_post) | **PUT** /apis/api.console.halo.run/v1alpha1/posts/{name} | 
[**update_post_content**](PostV1alpha1ConsoleApi.md#update_post_content) | **PUT** /apis/api.console.halo.run/v1alpha1/posts/{name}/content | 


# **delete_post_content**
> ContentWrapper delete_post_content(name, snapshot_name)

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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    snapshot_name = 'snapshot_name_example' # str | 

    try:
        api_response = api_instance.delete_post_content(name, snapshot_name)
        print("The response of PostV1alpha1ConsoleApi->delete_post_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->delete_post_content: %s\n" % e)
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

# **draft_post**
> Post draft_post(post_request)

Draft a post.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.post import Post
from halo_client.models.post_request import PostRequest
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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    post_request = halo_client.PostRequest() # PostRequest | 

    try:
        api_response = api_instance.draft_post(post_request)
        print("The response of PostV1alpha1ConsoleApi->draft_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->draft_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **post_request** | [**PostRequest**](PostRequest.md)|  | 

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

# **fetch_post_content**
> ContentWrapper fetch_post_content(name, snapshot_name)

Fetch content of post.

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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    snapshot_name = 'snapshot_name_example' # str | 

    try:
        api_response = api_instance.fetch_post_content(name, snapshot_name)
        print("The response of PostV1alpha1ConsoleApi->fetch_post_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->fetch_post_content: %s\n" % e)
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

# **fetch_post_head_content**
> ContentWrapper fetch_post_head_content(name)

Fetch head content of post.

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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.fetch_post_head_content(name)
        print("The response of PostV1alpha1ConsoleApi->fetch_post_head_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->fetch_post_head_content: %s\n" % e)
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

# **fetch_post_release_content**
> ContentWrapper fetch_post_release_content(name)

Fetch release content of post.

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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.fetch_post_release_content(name)
        print("The response of PostV1alpha1ConsoleApi->fetch_post_release_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->fetch_post_release_content: %s\n" % e)
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

# **list_post_snapshots**
> List[ListedSnapshotDto] list_post_snapshots(name)

List all snapshots for post content.

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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.list_post_snapshots(name)
        print("The response of PostV1alpha1ConsoleApi->list_post_snapshots:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->list_post_snapshots: %s\n" % e)
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

# **list_posts**
> ListedPostList list_posts(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort, publish_phase=publish_phase, keyword=keyword, category_with_children=category_with_children)

List posts.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.listed_post_list import ListedPostList
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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)
    publish_phase = 'publish_phase_example' # str | Posts filtered by publish phase. (optional)
    keyword = 'keyword_example' # str | Posts filtered by keyword. (optional)
    category_with_children = 'category_with_children_example' # str | Posts filtered by category including sub-categories. (optional)

    try:
        api_response = api_instance.list_posts(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort, publish_phase=publish_phase, keyword=keyword, category_with_children=category_with_children)
        print("The response of PostV1alpha1ConsoleApi->list_posts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->list_posts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**| Page number. Default is 0. | [optional] 
 **size** | **int**| Size number. Default is 0. | [optional] 
 **label_selector** | [**List[str]**](str.md)| Label selector. e.g.: hidden!&#x3D;true | [optional] 
 **field_selector** | [**List[str]**](str.md)| Field selector. e.g.: metadata.name&#x3D;&#x3D;halo | [optional] 
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 
 **publish_phase** | **str**| Posts filtered by publish phase. | [optional] 
 **keyword** | **str**| Posts filtered by keyword. | [optional] 
 **category_with_children** | **str**| Posts filtered by category including sub-categories. | [optional] 

### Return type

[**ListedPostList**](ListedPostList.md)

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

# **publish_post**
> Post publish_post(name, head_snapshot=head_snapshot, var_async=var_async)

Publish a post.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    head_snapshot = 'head_snapshot_example' # str | Head snapshot name of content. (optional)
    var_async = True # bool |  (optional)

    try:
        api_response = api_instance.publish_post(name, head_snapshot=head_snapshot, var_async=var_async)
        print("The response of PostV1alpha1ConsoleApi->publish_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->publish_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **head_snapshot** | **str**| Head snapshot name of content. | [optional] 
 **var_async** | **bool**|  | [optional] 

### Return type

[**Post**](Post.md)

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

# **recycle_post**
> recycle_post(name)

Recycle a post.

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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_instance.recycle_post(name)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->recycle_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **revert_to_specified_snapshot_for_post**
> Post revert_to_specified_snapshot_for_post(name, revert_snapshot_for_post_param)

Revert to specified snapshot for post content.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.post import Post
from halo_client.models.revert_snapshot_for_post_param import RevertSnapshotForPostParam
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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    revert_snapshot_for_post_param = halo_client.RevertSnapshotForPostParam() # RevertSnapshotForPostParam | 

    try:
        api_response = api_instance.revert_to_specified_snapshot_for_post(name, revert_snapshot_for_post_param)
        print("The response of PostV1alpha1ConsoleApi->revert_to_specified_snapshot_for_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->revert_to_specified_snapshot_for_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **revert_snapshot_for_post_param** | [**RevertSnapshotForPostParam**](RevertSnapshotForPostParam.md)|  | 

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

# **unpublish_post**
> Post unpublish_post(name)

UnPublish a post.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.unpublish_post(name)
        print("The response of PostV1alpha1ConsoleApi->unpublish_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->unpublish_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

[**Post**](Post.md)

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

# **update_draft_post**
> Post update_draft_post(name, post_request)

Update a post.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.post import Post
from halo_client.models.post_request import PostRequest
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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    post_request = halo_client.PostRequest() # PostRequest | 

    try:
        api_response = api_instance.update_draft_post(name, post_request)
        print("The response of PostV1alpha1ConsoleApi->update_draft_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->update_draft_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **post_request** | [**PostRequest**](PostRequest.md)|  | 

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

# **update_post_content**
> Post update_post_content(name, content)

Update a post's content.

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
    api_instance = halo_client.PostV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    content = halo_client.Content() # Content | 

    try:
        api_response = api_instance.update_post_content(name, content)
        print("The response of PostV1alpha1ConsoleApi->update_post_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostV1alpha1ConsoleApi->update_post_content: %s\n" % e)
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

