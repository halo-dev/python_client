# halo_client.ExtensionPointDefinitionV1alpha1Api

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_extension_point_definition**](ExtensionPointDefinitionV1alpha1Api.md#create_extension_point_definition) | **POST** /apis/plugin.halo.run/v1alpha1/extensionpointdefinitions | 
[**delete_extension_point_definition**](ExtensionPointDefinitionV1alpha1Api.md#delete_extension_point_definition) | **DELETE** /apis/plugin.halo.run/v1alpha1/extensionpointdefinitions/{name} | 
[**get_extension_point_definition**](ExtensionPointDefinitionV1alpha1Api.md#get_extension_point_definition) | **GET** /apis/plugin.halo.run/v1alpha1/extensionpointdefinitions/{name} | 
[**list_extension_point_definition**](ExtensionPointDefinitionV1alpha1Api.md#list_extension_point_definition) | **GET** /apis/plugin.halo.run/v1alpha1/extensionpointdefinitions | 
[**patch_extension_point_definition**](ExtensionPointDefinitionV1alpha1Api.md#patch_extension_point_definition) | **PATCH** /apis/plugin.halo.run/v1alpha1/extensionpointdefinitions/{name} | 
[**update_extension_point_definition**](ExtensionPointDefinitionV1alpha1Api.md#update_extension_point_definition) | **PUT** /apis/plugin.halo.run/v1alpha1/extensionpointdefinitions/{name} | 


# **create_extension_point_definition**
> ExtensionPointDefinition create_extension_point_definition(extension_point_definition=extension_point_definition)

Create ExtensionPointDefinition

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.extension_point_definition import ExtensionPointDefinition
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
    api_instance = halo_client.ExtensionPointDefinitionV1alpha1Api(api_client)
    extension_point_definition = halo_client.ExtensionPointDefinition() # ExtensionPointDefinition | Fresh extensionpointdefinition (optional)

    try:
        api_response = api_instance.create_extension_point_definition(extension_point_definition=extension_point_definition)
        print("The response of ExtensionPointDefinitionV1alpha1Api->create_extension_point_definition:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExtensionPointDefinitionV1alpha1Api->create_extension_point_definition: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **extension_point_definition** | [**ExtensionPointDefinition**](ExtensionPointDefinition.md)| Fresh extensionpointdefinition | [optional] 

### Return type

[**ExtensionPointDefinition**](ExtensionPointDefinition.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response extensionpointdefinitions created just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_extension_point_definition**
> delete_extension_point_definition(name)

Delete ExtensionPointDefinition

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
    api_instance = halo_client.ExtensionPointDefinitionV1alpha1Api(api_client)
    name = 'name_example' # str | Name of extensionpointdefinition

    try:
        api_instance.delete_extension_point_definition(name)
    except Exception as e:
        print("Exception when calling ExtensionPointDefinitionV1alpha1Api->delete_extension_point_definition: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of extensionpointdefinition | 

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
**200** | Response extensionpointdefinition deleted just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_extension_point_definition**
> ExtensionPointDefinition get_extension_point_definition(name)

Get ExtensionPointDefinition

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.extension_point_definition import ExtensionPointDefinition
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
    api_instance = halo_client.ExtensionPointDefinitionV1alpha1Api(api_client)
    name = 'name_example' # str | Name of extensionpointdefinition

    try:
        api_response = api_instance.get_extension_point_definition(name)
        print("The response of ExtensionPointDefinitionV1alpha1Api->get_extension_point_definition:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExtensionPointDefinitionV1alpha1Api->get_extension_point_definition: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of extensionpointdefinition | 

### Return type

[**ExtensionPointDefinition**](ExtensionPointDefinition.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response single extensionpointdefinition |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_extension_point_definition**
> ExtensionPointDefinitionList list_extension_point_definition(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)

List ExtensionPointDefinition

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.extension_point_definition_list import ExtensionPointDefinitionList
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
    api_instance = halo_client.ExtensionPointDefinitionV1alpha1Api(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        api_response = api_instance.list_extension_point_definition(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)
        print("The response of ExtensionPointDefinitionV1alpha1Api->list_extension_point_definition:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExtensionPointDefinitionV1alpha1Api->list_extension_point_definition: %s\n" % e)
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

[**ExtensionPointDefinitionList**](ExtensionPointDefinitionList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response extensionpointdefinitions |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_extension_point_definition**
> ExtensionPointDefinition patch_extension_point_definition(name, json_patch_inner=json_patch_inner)

Patch ExtensionPointDefinition

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.extension_point_definition import ExtensionPointDefinition
from halo_client.models.json_patch_inner import JsonPatchInner
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
    api_instance = halo_client.ExtensionPointDefinitionV1alpha1Api(api_client)
    name = 'name_example' # str | Name of extensionpointdefinition
    json_patch_inner = [halo_client.JsonPatchInner()] # List[JsonPatchInner] |  (optional)

    try:
        api_response = api_instance.patch_extension_point_definition(name, json_patch_inner=json_patch_inner)
        print("The response of ExtensionPointDefinitionV1alpha1Api->patch_extension_point_definition:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExtensionPointDefinitionV1alpha1Api->patch_extension_point_definition: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of extensionpointdefinition | 
 **json_patch_inner** | [**List[JsonPatchInner]**](JsonPatchInner.md)|  | [optional] 

### Return type

[**ExtensionPointDefinition**](ExtensionPointDefinition.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json-patch+json
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response extensionpointdefinition patched just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_extension_point_definition**
> ExtensionPointDefinition update_extension_point_definition(name, extension_point_definition=extension_point_definition)

Update ExtensionPointDefinition

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.extension_point_definition import ExtensionPointDefinition
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
    api_instance = halo_client.ExtensionPointDefinitionV1alpha1Api(api_client)
    name = 'name_example' # str | Name of extensionpointdefinition
    extension_point_definition = halo_client.ExtensionPointDefinition() # ExtensionPointDefinition | Updated extensionpointdefinition (optional)

    try:
        api_response = api_instance.update_extension_point_definition(name, extension_point_definition=extension_point_definition)
        print("The response of ExtensionPointDefinitionV1alpha1Api->update_extension_point_definition:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExtensionPointDefinitionV1alpha1Api->update_extension_point_definition: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Name of extensionpointdefinition | 
 **extension_point_definition** | [**ExtensionPointDefinition**](ExtensionPointDefinition.md)| Updated extensionpointdefinition | [optional] 

### Return type

[**ExtensionPointDefinition**](ExtensionPointDefinition.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Response extensionpointdefinitions updated just now |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

