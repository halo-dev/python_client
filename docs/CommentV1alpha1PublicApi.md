# halo_client.CommentV1alpha1PublicApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_comment1**](CommentV1alpha1PublicApi.md#create_comment1) | **POST** /apis/api.halo.run/v1alpha1/comments | 
[**create_reply1**](CommentV1alpha1PublicApi.md#create_reply1) | **POST** /apis/api.halo.run/v1alpha1/comments/{name}/reply | 
[**get_comment**](CommentV1alpha1PublicApi.md#get_comment) | **GET** /apis/api.halo.run/v1alpha1/comments/{name} | 
[**list_comment_replies**](CommentV1alpha1PublicApi.md#list_comment_replies) | **GET** /apis/api.halo.run/v1alpha1/comments/{name}/reply | 
[**list_comments1**](CommentV1alpha1PublicApi.md#list_comments1) | **GET** /apis/api.halo.run/v1alpha1/comments | 


# **create_comment1**
> Comment create_comment1(comment_request)

Create a comment.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.comment import Comment
from halo_client.models.comment_request import CommentRequest
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
    api_instance = halo_client.CommentV1alpha1PublicApi(api_client)
    comment_request = halo_client.CommentRequest() # CommentRequest | 

    try:
        api_response = api_instance.create_comment1(comment_request)
        print("The response of CommentV1alpha1PublicApi->create_comment1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommentV1alpha1PublicApi->create_comment1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **comment_request** | [**CommentRequest**](CommentRequest.md)|  | 

### Return type

[**Comment**](Comment.md)

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

# **create_reply1**
> Reply create_reply1(name, reply_request)

Create a reply.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.reply import Reply
from halo_client.models.reply_request import ReplyRequest
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
    api_instance = halo_client.CommentV1alpha1PublicApi(api_client)
    name = 'name_example' # str | 
    reply_request = halo_client.ReplyRequest() # ReplyRequest | 

    try:
        api_response = api_instance.create_reply1(name, reply_request)
        print("The response of CommentV1alpha1PublicApi->create_reply1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommentV1alpha1PublicApi->create_reply1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **reply_request** | [**ReplyRequest**](ReplyRequest.md)|  | 

### Return type

[**Reply**](Reply.md)

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

# **get_comment**
> CommentVoList get_comment(name)

Get a comment.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.comment_vo_list import CommentVoList
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
    api_instance = halo_client.CommentV1alpha1PublicApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.get_comment(name)
        print("The response of CommentV1alpha1PublicApi->get_comment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommentV1alpha1PublicApi->get_comment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

[**CommentVoList**](CommentVoList.md)

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

# **list_comment_replies**
> ReplyVoList list_comment_replies(name, page=page, size=size)

List comment replies.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.reply_vo_list import ReplyVoList
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
    api_instance = halo_client.CommentV1alpha1PublicApi(api_client)
    name = 'name_example' # str | 
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)

    try:
        api_response = api_instance.list_comment_replies(name, page=page, size=size)
        print("The response of CommentV1alpha1PublicApi->list_comment_replies:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommentV1alpha1PublicApi->list_comment_replies: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **page** | **int**| Page number. Default is 0. | [optional] 
 **size** | **int**| Size number. Default is 0. | [optional] 

### Return type

[**ReplyVoList**](ReplyVoList.md)

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

# **list_comments1**
> CommentWithReplyVoList list_comments1(version, kind, name, page=page, size=size, sort=sort, group=group, with_replies=with_replies, reply_size=reply_size)

List comments.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.comment_with_reply_vo_list import CommentWithReplyVoList
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
    api_instance = halo_client.CommentV1alpha1PublicApi(api_client)
    version = 'version_example' # str | The comment subject version.
    kind = 'kind_example' # str | The comment subject kind.
    name = 'name_example' # str | The comment subject name.
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)
    group = 'group_example' # str | The comment subject group. (optional)
    with_replies = True # bool | Whether to include replies. Default is false. (optional)
    reply_size = 56 # int | Reply size of the comment, default is 10, only works when withReplies is true. (optional)

    try:
        api_response = api_instance.list_comments1(version, kind, name, page=page, size=size, sort=sort, group=group, with_replies=with_replies, reply_size=reply_size)
        print("The response of CommentV1alpha1PublicApi->list_comments1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommentV1alpha1PublicApi->list_comments1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **version** | **str**| The comment subject version. | 
 **kind** | **str**| The comment subject kind. | 
 **name** | **str**| The comment subject name. | 
 **page** | **int**| Page number. Default is 0. | [optional] 
 **size** | **int**| Size number. Default is 0. | [optional] 
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 
 **group** | **str**| The comment subject group. | [optional] 
 **with_replies** | **bool**| Whether to include replies. Default is false. | [optional] 
 **reply_size** | **int**| Reply size of the comment, default is 10, only works when withReplies is true. | [optional] 

### Return type

[**CommentWithReplyVoList**](CommentWithReplyVoList.md)

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

