# halo_client.PersonalAccessTokenV1alpha1Api

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_personal_access_token**](PersonalAccessTokenV1alpha1Api.md#create_personal_access_token) | **POST** /apis/security.halo.run/v1alpha1/personalaccesstokens | 
[**delete_personal_access_token**](PersonalAccessTokenV1alpha1Api.md#delete_personal_access_token) | **DELETE** /apis/security.halo.run/v1alpha1/personalaccesstokens/{name} | 
[**get_personal_access_token**](PersonalAccessTokenV1alpha1Api.md#get_personal_access_token) | **GET** /apis/security.halo.run/v1alpha1/personalaccesstokens/{name} | 
[**list_personal_access_token**](PersonalAccessTokenV1alpha1Api.md#list_personal_access_token) | **GET** /apis/security.halo.run/v1alpha1/personalaccesstokens | 
[**patch_personal_access_token**](PersonalAccessTokenV1alpha1Api.md#patch_personal_access_token) | **PATCH** /apis/security.halo.run/v1alpha1/personalaccesstokens/{name} | 
[**update_personal_access_token**](PersonalAccessTokenV1alpha1Api.md#update_personal_access_token) | **PUT** /apis/security.halo.run/v1alpha1/personalaccesstokens/{name} | 


# **create_personal_access_token**
> PersonalAccessToken create_personal_access_token(personal_access_token=personal_access_token)

Create PersonalAccessToken

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.personal_access_token import PersonalAccessToken
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
    api_instance = halo_client.PersonalAccessTokenV1alpha1Api(api_client)
    personal_access_token = halo_client.PersonalAccessToken() # PersonalAccessToken | Fresh personalaccesstoken (optional)

    try:
        api_response = api_instance.create_personal_access_token(personal_access_token=personal_access_token)
        print("The response of PersonalAccessTokenV1alpha1Api->create_personal_access_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PersonalAccessTokenV1alpha1Api->create_personal_access_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **personal_access_token** | [**PersonalAccessToken**](PersonalAccessToken.md)| Fresh personalaccesstoken | [optional] 

### Return type

[**PersonalAccessToken**](PersonalAccessToken.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response personalaccesstokens created just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_personal_access_token**
> delete_personal_access_token(name)

Delete PersonalAccessToken

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
    api_instance = halo_client.PersonalAccessTokenV1alpha1Api(api_client)
    name = 'name_example' # str | Name of personalaccesstoken

    try:
        api_instance.delete_personal_access_token(name)
    except Exception as e:
        print("Exception when calling PersonalAccessTokenV1alpha1Api->delete_personal_access_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of personalaccesstoken | 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response personalaccesstoken deleted just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_personal_access_token**
> PersonalAccessToken get_personal_access_token(name)

Get PersonalAccessToken

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.personal_access_token import PersonalAccessToken
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
    api_instance = halo_client.PersonalAccessTokenV1alpha1Api(api_client)
    name = 'name_example' # str | Name of personalaccesstoken

    try:
        api_response = api_instance.get_personal_access_token(name)
        print("The response of PersonalAccessTokenV1alpha1Api->get_personal_access_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PersonalAccessTokenV1alpha1Api->get_personal_access_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of personalaccesstoken | 

### Return type

[**PersonalAccessToken**](PersonalAccessToken.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response single personalaccesstoken |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_personal_access_token**
> PersonalAccessTokenList list_personal_access_token(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)

List PersonalAccessToken

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.personal_access_token_list import PersonalAccessTokenList
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
    api_instance = halo_client.PersonalAccessTokenV1alpha1Api(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        api_response = api_instance.list_personal_access_token(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)
        print("The response of PersonalAccessTokenV1alpha1Api->list_personal_access_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PersonalAccessTokenV1alpha1Api->list_personal_access_token: %s\n" % e)
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

[**PersonalAccessTokenList**](PersonalAccessTokenList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response personalaccesstokens |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_personal_access_token**
> PersonalAccessToken patch_personal_access_token(name, json_patch_inner=json_patch_inner)

Patch PersonalAccessToken

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.json_patch_inner import JsonPatchInner
from halo_client.models.personal_access_token import PersonalAccessToken
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
    api_instance = halo_client.PersonalAccessTokenV1alpha1Api(api_client)
    name = 'name_example' # str | Name of personalaccesstoken
    json_patch_inner = [halo_client.JsonPatchInner()] # List[JsonPatchInner] |  (optional)

    try:
        api_response = api_instance.patch_personal_access_token(name, json_patch_inner=json_patch_inner)
        print("The response of PersonalAccessTokenV1alpha1Api->patch_personal_access_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PersonalAccessTokenV1alpha1Api->patch_personal_access_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of personalaccesstoken | 
 **json_patch_inner** | [**List[JsonPatchInner]**](JsonPatchInner.md)|  | [optional] 

### Return type

[**PersonalAccessToken**](PersonalAccessToken.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json-patch+json
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response personalaccesstoken patched just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_personal_access_token**
> PersonalAccessToken update_personal_access_token(name, personal_access_token=personal_access_token)

Update PersonalAccessToken

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.personal_access_token import PersonalAccessToken
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
    api_instance = halo_client.PersonalAccessTokenV1alpha1Api(api_client)
    name = 'name_example' # str | Name of personalaccesstoken
    personal_access_token = halo_client.PersonalAccessToken() # PersonalAccessToken | Updated personalaccesstoken (optional)

    try:
        api_response = api_instance.update_personal_access_token(name, personal_access_token=personal_access_token)
        print("The response of PersonalAccessTokenV1alpha1Api->update_personal_access_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PersonalAccessTokenV1alpha1Api->update_personal_access_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of personalaccesstoken | 
 **personal_access_token** | [**PersonalAccessToken**](PersonalAccessToken.md)| Updated personalaccesstoken | [optional] 

### Return type

[**PersonalAccessToken**](PersonalAccessToken.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response personalaccesstokens updated just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

