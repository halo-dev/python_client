# halo_client.PluginV1alpha1ConsoleApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**change_plugin_running_state**](PluginV1alpha1ConsoleApi.md#change_plugin_running_state) | **PUT** /apis/api.console.halo.run/v1alpha1/plugins/{name}/plugin-state | 
[**fetch_css_bundle**](PluginV1alpha1ConsoleApi.md#fetch_css_bundle) | **GET** /apis/api.console.halo.run/v1alpha1/plugins/-/bundle.css | 
[**fetch_js_bundle**](PluginV1alpha1ConsoleApi.md#fetch_js_bundle) | **GET** /apis/api.console.halo.run/v1alpha1/plugins/-/bundle.js | 
[**fetch_plugin_json_config**](PluginV1alpha1ConsoleApi.md#fetch_plugin_json_config) | **GET** /apis/api.console.halo.run/v1alpha1/plugins/{name}/json-config | 
[**fetch_plugin_setting**](PluginV1alpha1ConsoleApi.md#fetch_plugin_setting) | **GET** /apis/api.console.halo.run/v1alpha1/plugins/{name}/setting | 
[**install_plugin**](PluginV1alpha1ConsoleApi.md#install_plugin) | **POST** /apis/api.console.halo.run/v1alpha1/plugins/install | 
[**install_plugin_from_uri**](PluginV1alpha1ConsoleApi.md#install_plugin_from_uri) | **POST** /apis/api.console.halo.run/v1alpha1/plugins/-/install-from-uri | 
[**list_plugins**](PluginV1alpha1ConsoleApi.md#list_plugins) | **GET** /apis/api.console.halo.run/v1alpha1/plugins | 
[**reload_plugin**](PluginV1alpha1ConsoleApi.md#reload_plugin) | **PUT** /apis/api.console.halo.run/v1alpha1/plugins/{name}/reload | 
[**reset_plugin_config**](PluginV1alpha1ConsoleApi.md#reset_plugin_config) | **PUT** /apis/api.console.halo.run/v1alpha1/plugins/{name}/reset-config | 
[**update_plugin_json_config**](PluginV1alpha1ConsoleApi.md#update_plugin_json_config) | **PUT** /apis/api.console.halo.run/v1alpha1/plugins/{name}/json-config | 
[**upgrade_plugin**](PluginV1alpha1ConsoleApi.md#upgrade_plugin) | **POST** /apis/api.console.halo.run/v1alpha1/plugins/{name}/upgrade | 
[**upgrade_plugin_from_uri**](PluginV1alpha1ConsoleApi.md#upgrade_plugin_from_uri) | **POST** /apis/api.console.halo.run/v1alpha1/plugins/{name}/upgrade-from-uri | 


# **change_plugin_running_state**
> Plugin change_plugin_running_state(name, plugin_running_state_request)

Change the running state of a plugin by name.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.plugin import Plugin
from halo_client.models.plugin_running_state_request import PluginRunningStateRequest
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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    plugin_running_state_request = halo_client.PluginRunningStateRequest() # PluginRunningStateRequest | 

    try:
        api_response = api_instance.change_plugin_running_state(name, plugin_running_state_request)
        print("The response of PluginV1alpha1ConsoleApi->change_plugin_running_state:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->change_plugin_running_state: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **plugin_running_state_request** | [**PluginRunningStateRequest**](PluginRunningStateRequest.md)|  | 

### Return type

[**Plugin**](Plugin.md)

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

# **fetch_css_bundle**
> str fetch_css_bundle()

Merge all CSS bundles of enabled plugins into one.

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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)

    try:
        api_response = api_instance.fetch_css_bundle()
        print("The response of PluginV1alpha1ConsoleApi->fetch_css_bundle:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->fetch_css_bundle: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**str**

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

# **fetch_js_bundle**
> str fetch_js_bundle()

Merge all JS bundles of enabled plugins into one.

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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)

    try:
        api_response = api_instance.fetch_js_bundle()
        print("The response of PluginV1alpha1ConsoleApi->fetch_js_bundle:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->fetch_js_bundle: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**str**

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

# **fetch_plugin_json_config**
> object fetch_plugin_json_config(name)

Fetch converted json config of plugin by configured configMapName.

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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.fetch_plugin_json_config(name)
        print("The response of PluginV1alpha1ConsoleApi->fetch_plugin_json_config:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->fetch_plugin_json_config: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

**object**

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

# **fetch_plugin_setting**
> Setting fetch_plugin_setting(name)

Fetch setting of plugin.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.setting import Setting
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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.fetch_plugin_setting(name)
        print("The response of PluginV1alpha1ConsoleApi->fetch_plugin_setting:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->fetch_plugin_setting: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

[**Setting**](Setting.md)

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

# **install_plugin**
> Plugin install_plugin(file=file, preset_name=preset_name, source=source)

Install a plugin by uploading a Jar file.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.plugin import Plugin
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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)
    file = None # bytearray |  (optional)
    preset_name = 'preset_name_example' # str | Plugin preset name. We will find the plugin from plugin presets (optional)
    source = 'source_example' # str | Install source. Default is file. (optional)

    try:
        api_response = api_instance.install_plugin(file=file, preset_name=preset_name, source=source)
        print("The response of PluginV1alpha1ConsoleApi->install_plugin:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->install_plugin: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | **bytearray**|  | [optional] 
 **preset_name** | **str**| Plugin preset name. We will find the plugin from plugin presets | [optional] 
 **source** | **str**| Install source. Default is file. | [optional] 

### Return type

[**Plugin**](Plugin.md)

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

# **install_plugin_from_uri**
> Plugin install_plugin_from_uri(install_from_uri_request)

Install a plugin from uri.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.install_from_uri_request import InstallFromUriRequest
from halo_client.models.plugin import Plugin
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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)
    install_from_uri_request = halo_client.InstallFromUriRequest() # InstallFromUriRequest | 

    try:
        api_response = api_instance.install_plugin_from_uri(install_from_uri_request)
        print("The response of PluginV1alpha1ConsoleApi->install_plugin_from_uri:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->install_plugin_from_uri: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **install_from_uri_request** | [**InstallFromUriRequest**](InstallFromUriRequest.md)|  | 

### Return type

[**Plugin**](Plugin.md)

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

# **list_plugins**
> PluginList list_plugins(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort, keyword=keyword, enabled=enabled)

List plugins using query criteria and sort params

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.plugin_list import PluginList
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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)
    keyword = 'keyword_example' # str | Keyword of plugin name or description (optional)
    enabled = True # bool | Whether the plugin is enabled (optional)

    try:
        api_response = api_instance.list_plugins(page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort, keyword=keyword, enabled=enabled)
        print("The response of PluginV1alpha1ConsoleApi->list_plugins:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->list_plugins: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**| Page number. Default is 0. | [optional] 
 **size** | **int**| Size number. Default is 0. | [optional] 
 **label_selector** | [**List[str]**](str.md)| Label selector. e.g.: hidden!&#x3D;true | [optional] 
 **field_selector** | [**List[str]**](str.md)| Field selector. e.g.: metadata.name&#x3D;&#x3D;halo | [optional] 
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 
 **keyword** | **str**| Keyword of plugin name or description | [optional] 
 **enabled** | **bool**| Whether the plugin is enabled | [optional] 

### Return type

[**PluginList**](PluginList.md)

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

# **reload_plugin**
> Plugin reload_plugin(name)

Reload a plugin by name.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.plugin import Plugin
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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.reload_plugin(name)
        print("The response of PluginV1alpha1ConsoleApi->reload_plugin:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->reload_plugin: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

[**Plugin**](Plugin.md)

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

# **reset_plugin_config**
> ConfigMap reset_plugin_config(name)

Reset the configMap of plugin setting.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.config_map import ConfigMap
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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 

    try:
        api_response = api_instance.reset_plugin_config(name)
        print("The response of PluginV1alpha1ConsoleApi->reset_plugin_config:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->reset_plugin_config: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 

### Return type

[**ConfigMap**](ConfigMap.md)

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

# **update_plugin_json_config**
> update_plugin_json_config(name, body)

Update the config of plugin setting.

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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    body = None # object | 

    try:
        api_instance.update_plugin_json_config(name, body)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->update_plugin_json_config: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **body** | **object**|  | 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | No Content |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upgrade_plugin**
> upgrade_plugin(name, file=file, preset_name=preset_name, source=source)

Upgrade a plugin by uploading a Jar file

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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    file = None # bytearray |  (optional)
    preset_name = 'preset_name_example' # str | Plugin preset name. We will find the plugin from plugin presets (optional)
    source = 'source_example' # str | Install source. Default is file. (optional)

    try:
        api_instance.upgrade_plugin(name, file=file, preset_name=preset_name, source=source)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->upgrade_plugin: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **file** | **bytearray**|  | [optional] 
 **preset_name** | **str**| Plugin preset name. We will find the plugin from plugin presets | [optional] 
 **source** | **str**| Install source. Default is file. | [optional] 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined


[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upgrade_plugin_from_uri**
> Plugin upgrade_plugin_from_uri(name, upgrade_from_uri_request)

Upgrade a plugin from uri.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.plugin import Plugin
from halo_client.models.upgrade_from_uri_request import UpgradeFromUriRequest
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
    api_instance = halo_client.PluginV1alpha1ConsoleApi(api_client)
    name = 'name_example' # str | 
    upgrade_from_uri_request = halo_client.UpgradeFromUriRequest() # UpgradeFromUriRequest | 

    try:
        api_response = api_instance.upgrade_plugin_from_uri(name, upgrade_from_uri_request)
        print("The response of PluginV1alpha1ConsoleApi->upgrade_plugin_from_uri:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PluginV1alpha1ConsoleApi->upgrade_plugin_from_uri: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | 
 **upgrade_from_uri_request** | [**UpgradeFromUriRequest**](UpgradeFromUriRequest.md)|  | 

### Return type

[**Plugin**](Plugin.md)

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

