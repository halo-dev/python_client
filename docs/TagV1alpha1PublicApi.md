# halo_client.TagV1alpha1PublicApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**query_posts_by_tag_name**](TagV1alpha1PublicApi.md#query_posts_by_tag_name) | **GET** /apis/api.content.halo.run/v1alpha1/tags/{name}/posts | 
[**query_tag_by_name**](TagV1alpha1PublicApi.md#query_tag_by_name) | **GET** /apis/api.content.halo.run/v1alpha1/tags/{name} | 
[**query_tags**](TagV1alpha1PublicApi.md#query_tags) | **GET** /apis/api.content.halo.run/v1alpha1/tags | 


# **query_posts_by_tag_name**
> ListedPostVo query_posts_by_tag_name(name, page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)

Lists posts by tag name

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.listed_post_vo import ListedPostVo
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
    api_instance = halo_client.TagV1alpha1PublicApi(api_client)
    name = 'name_example' # str | Tag name
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        api_response = api_instance.query_posts_by_tag_name(name, page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)
        print("The response of TagV1alpha1PublicApi->query_posts_by_tag_name:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TagV1alpha1PublicApi->query_posts_by_tag_name: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Tag name | 
 **page** | **int**| Page number. Default is 0. | [optional] 
 **size** | **int**| Size number. Default is 0. | [optional] 
 **label_selector** | [**List[str]**](str.md)| Label selector. e.g.: hidden!&#x3D;true | [optional] 
 **field_selector** | [**List[str]**](str.md)| Field selector. e.g.: metadata.name&#x3D;&#x3D;halo | [optional] 
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 

### Return type

[**ListedPostVo**](ListedPostVo.md)

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

# **query_tag_by_name**
> TagVo query_tag_by_name(name)

Gets tag by name

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.tag_vo import TagVo
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
    api_instance = halo_client.TagV1alpha1PublicApi(api_client)
    name = 'name_example' # str | Tag name

    try:
        api_response = api_instance.query_tag_by_name(name)
        print("The response of TagV1alpha1PublicApi->query_tag_by_name:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TagV1alpha1PublicApi->query_tag_by_name: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Tag name | 

### Return type

[**TagVo**](TagVo.md)

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

# **query_tags**
> TagVoList query_tags(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)

Lists tags

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.tag_vo_list import TagVoList
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
    api_instance = halo_client.TagV1alpha1PublicApi(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        api_response = api_instance.query_tags(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)
        print("The response of TagV1alpha1PublicApi->query_tags:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TagV1alpha1PublicApi->query_tags: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**| Page number. Default is 0. | [optional] 
 **size** | **int**| Size number. Default is 0. | [optional] 
 **label_selector** | [**List[str]**](str.md)| Label selector. e.g.: hidden!&#x3D;true | [optional] 
 **field_selector** | [**List[str]**](str.md)| Field selector. e.g.: metadata.name&#x3D;&#x3D;halo | [optional] 
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 

### Return type

[**TagVoList**](TagVoList.md)

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

