# halo_client.NotificationV1alpha1UcApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_specified_notification**](NotificationV1alpha1UcApi.md#delete_specified_notification) | **DELETE** /apis/api.notification.halo.run/v1alpha1/userspaces/{username}/notifications/{name} | 
[**list_user_notification_preferences**](NotificationV1alpha1UcApi.md#list_user_notification_preferences) | **GET** /apis/api.notification.halo.run/v1alpha1/userspaces/{username}/notification-preferences | 
[**list_user_notifications**](NotificationV1alpha1UcApi.md#list_user_notifications) | **GET** /apis/api.notification.halo.run/v1alpha1/userspaces/{username}/notifications | 
[**mark_notification_as_read**](NotificationV1alpha1UcApi.md#mark_notification_as_read) | **PUT** /apis/api.notification.halo.run/v1alpha1/userspaces/{username}/notifications/{name}/mark-as-read | 
[**mark_notifications_as_read**](NotificationV1alpha1UcApi.md#mark_notifications_as_read) | **PUT** /apis/api.notification.halo.run/v1alpha1/userspaces/{username}/notifications/-/mark-specified-as-read | 
[**save_user_notification_preferences**](NotificationV1alpha1UcApi.md#save_user_notification_preferences) | **POST** /apis/api.notification.halo.run/v1alpha1/userspaces/{username}/notification-preferences | 


# **delete_specified_notification**
> Notification delete_specified_notification(username, name)

Delete the specified notification.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.notification import Notification
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
    api_instance = halo_client.NotificationV1alpha1UcApi(api_client)
    username = 'username_example' # str | Username
    name = 'name_example' # str | Notification name

    try:
        api_response = api_instance.delete_specified_notification(username, name)
        print("The response of NotificationV1alpha1UcApi->delete_specified_notification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationV1alpha1UcApi->delete_specified_notification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **username** | **str**| Username | 
 **name** | **str**| Notification name | 

### Return type

[**Notification**](Notification.md)

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

# **list_user_notification_preferences**
> ReasonTypeNotifierMatrix list_user_notification_preferences(username)

List notification preferences for the authenticated user.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.reason_type_notifier_matrix import ReasonTypeNotifierMatrix
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
    api_instance = halo_client.NotificationV1alpha1UcApi(api_client)
    username = 'username_example' # str | Username

    try:
        api_response = api_instance.list_user_notification_preferences(username)
        print("The response of NotificationV1alpha1UcApi->list_user_notification_preferences:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationV1alpha1UcApi->list_user_notification_preferences: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **username** | **str**| Username | 

### Return type

[**ReasonTypeNotifierMatrix**](ReasonTypeNotifierMatrix.md)

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

# **list_user_notifications**
> NotificationList list_user_notifications(username, page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)

List notifications for the authenticated user.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.notification_list import NotificationList
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
    api_instance = halo_client.NotificationV1alpha1UcApi(api_client)
    username = 'username_example' # str | Username
    page = 56 # int | Page number. Default is 0. (optional)
    size = 56 # int | Size number. Default is 0. (optional)
    label_selector = ['label_selector_example'] # List[str] | Label selector. e.g.: hidden!=true (optional)
    field_selector = ['field_selector_example'] # List[str] | Field selector. e.g.: metadata.name==halo (optional)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        api_response = api_instance.list_user_notifications(username, page=page, size=size, label_selector=label_selector, field_selector=field_selector, sort=sort)
        print("The response of NotificationV1alpha1UcApi->list_user_notifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationV1alpha1UcApi->list_user_notifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **username** | **str**| Username | 
 **page** | **int**| Page number. Default is 0. | [optional] 
 **size** | **int**| Size number. Default is 0. | [optional] 
 **label_selector** | [**List[str]**](str.md)| Label selector. e.g.: hidden!&#x3D;true | [optional] 
 **field_selector** | [**List[str]**](str.md)| Field selector. e.g.: metadata.name&#x3D;&#x3D;halo | [optional] 
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 

### Return type

[**NotificationList**](NotificationList.md)

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

# **mark_notification_as_read**
> Notification mark_notification_as_read(username, name)

Mark the specified notification as read.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.notification import Notification
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
    api_instance = halo_client.NotificationV1alpha1UcApi(api_client)
    username = 'username_example' # str | Username
    name = 'name_example' # str | Notification name

    try:
        api_response = api_instance.mark_notification_as_read(username, name)
        print("The response of NotificationV1alpha1UcApi->mark_notification_as_read:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationV1alpha1UcApi->mark_notification_as_read: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **username** | **str**| Username | 
 **name** | **str**| Notification name | 

### Return type

[**Notification**](Notification.md)

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

# **mark_notifications_as_read**
> List[str] mark_notifications_as_read(username, mark_specified_request)

Mark the specified notifications as read.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.mark_specified_request import MarkSpecifiedRequest
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
    api_instance = halo_client.NotificationV1alpha1UcApi(api_client)
    username = 'username_example' # str | Username
    mark_specified_request = halo_client.MarkSpecifiedRequest() # MarkSpecifiedRequest | 

    try:
        api_response = api_instance.mark_notifications_as_read(username, mark_specified_request)
        print("The response of NotificationV1alpha1UcApi->mark_notifications_as_read:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationV1alpha1UcApi->mark_notifications_as_read: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **username** | **str**| Username | 
 **mark_specified_request** | [**MarkSpecifiedRequest**](MarkSpecifiedRequest.md)|  | 

### Return type

**List[str]**

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

# **save_user_notification_preferences**
> ReasonTypeNotifierMatrix save_user_notification_preferences(username, reason_type_notifier_collection_request=reason_type_notifier_collection_request)

Save notification preferences for the authenticated user.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.reason_type_notifier_collection_request import ReasonTypeNotifierCollectionRequest
from halo_client.models.reason_type_notifier_matrix import ReasonTypeNotifierMatrix
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
    api_instance = halo_client.NotificationV1alpha1UcApi(api_client)
    username = 'username_example' # str | Username
    reason_type_notifier_collection_request = halo_client.ReasonTypeNotifierCollectionRequest() # ReasonTypeNotifierCollectionRequest |  (optional)

    try:
        api_response = api_instance.save_user_notification_preferences(username, reason_type_notifier_collection_request=reason_type_notifier_collection_request)
        print("The response of NotificationV1alpha1UcApi->save_user_notification_preferences:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationV1alpha1UcApi->save_user_notification_preferences: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **username** | **str**| Username | 
 **reason_type_notifier_collection_request** | [**ReasonTypeNotifierCollectionRequest**](ReasonTypeNotifierCollectionRequest.md)|  | [optional] 

### Return type

[**ReasonTypeNotifierMatrix**](ReasonTypeNotifierMatrix.md)

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

