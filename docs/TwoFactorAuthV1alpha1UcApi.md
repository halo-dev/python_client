# halo_client.TwoFactorAuthV1alpha1UcApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**configurer_totp**](TwoFactorAuthV1alpha1UcApi.md#configurer_totp) | **POST** /apis/uc.api.security.halo.run/v1alpha1/authentications/two-factor/totp | 
[**delete_totp**](TwoFactorAuthV1alpha1UcApi.md#delete_totp) | **DELETE** /apis/uc.api.security.halo.run/v1alpha1/authentications/two-factor/totp/- | 
[**disable_two_factor**](TwoFactorAuthV1alpha1UcApi.md#disable_two_factor) | **PUT** /apis/uc.api.security.halo.run/v1alpha1/authentications/two-factor/settings/disabled | 
[**enable_two_factor**](TwoFactorAuthV1alpha1UcApi.md#enable_two_factor) | **PUT** /apis/uc.api.security.halo.run/v1alpha1/authentications/two-factor/settings/enabled | 
[**get_totp_auth_link**](TwoFactorAuthV1alpha1UcApi.md#get_totp_auth_link) | **GET** /apis/uc.api.security.halo.run/v1alpha1/authentications/two-factor/totp/auth-link | 
[**get_two_factor_authentication_settings**](TwoFactorAuthV1alpha1UcApi.md#get_two_factor_authentication_settings) | **GET** /apis/uc.api.security.halo.run/v1alpha1/authentications/two-factor/settings | 


# **configurer_totp**
> TwoFactorAuthSettings configurer_totp(totp_request=totp_request)

Configure a TOTP

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.totp_request import TotpRequest
from halo_client.models.two_factor_auth_settings import TwoFactorAuthSettings
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
    api_instance = halo_client.TwoFactorAuthV1alpha1UcApi(api_client)
    totp_request = halo_client.TotpRequest() # TotpRequest |  (optional)

    try:
        api_response = api_instance.configurer_totp(totp_request=totp_request)
        print("The response of TwoFactorAuthV1alpha1UcApi->configurer_totp:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwoFactorAuthV1alpha1UcApi->configurer_totp: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **totp_request** | [**TotpRequest**](TotpRequest.md)|  | [optional] 

### Return type

[**TwoFactorAuthSettings**](TwoFactorAuthSettings.md)

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

# **delete_totp**
> TwoFactorAuthSettings delete_totp(password_request=password_request)

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.password_request import PasswordRequest
from halo_client.models.two_factor_auth_settings import TwoFactorAuthSettings
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
    api_instance = halo_client.TwoFactorAuthV1alpha1UcApi(api_client)
    password_request = halo_client.PasswordRequest() # PasswordRequest |  (optional)

    try:
        api_response = api_instance.delete_totp(password_request=password_request)
        print("The response of TwoFactorAuthV1alpha1UcApi->delete_totp:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwoFactorAuthV1alpha1UcApi->delete_totp: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **password_request** | [**PasswordRequest**](PasswordRequest.md)|  | [optional] 

### Return type

[**TwoFactorAuthSettings**](TwoFactorAuthSettings.md)

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

# **disable_two_factor**
> TwoFactorAuthSettings disable_two_factor(password_request=password_request)

Disable Two-factor authentication

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.password_request import PasswordRequest
from halo_client.models.two_factor_auth_settings import TwoFactorAuthSettings
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
    api_instance = halo_client.TwoFactorAuthV1alpha1UcApi(api_client)
    password_request = halo_client.PasswordRequest() # PasswordRequest |  (optional)

    try:
        api_response = api_instance.disable_two_factor(password_request=password_request)
        print("The response of TwoFactorAuthV1alpha1UcApi->disable_two_factor:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwoFactorAuthV1alpha1UcApi->disable_two_factor: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **password_request** | [**PasswordRequest**](PasswordRequest.md)|  | [optional] 

### Return type

[**TwoFactorAuthSettings**](TwoFactorAuthSettings.md)

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

# **enable_two_factor**
> TwoFactorAuthSettings enable_two_factor(password_request=password_request)

Enable Two-factor authentication

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.password_request import PasswordRequest
from halo_client.models.two_factor_auth_settings import TwoFactorAuthSettings
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
    api_instance = halo_client.TwoFactorAuthV1alpha1UcApi(api_client)
    password_request = halo_client.PasswordRequest() # PasswordRequest |  (optional)

    try:
        api_response = api_instance.enable_two_factor(password_request=password_request)
        print("The response of TwoFactorAuthV1alpha1UcApi->enable_two_factor:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwoFactorAuthV1alpha1UcApi->enable_two_factor: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **password_request** | [**PasswordRequest**](PasswordRequest.md)|  | [optional] 

### Return type

[**TwoFactorAuthSettings**](TwoFactorAuthSettings.md)

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

# **get_totp_auth_link**
> TotpAuthLinkResponse get_totp_auth_link()

Get TOTP auth link, including secret

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.totp_auth_link_response import TotpAuthLinkResponse
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
    api_instance = halo_client.TwoFactorAuthV1alpha1UcApi(api_client)

    try:
        api_response = api_instance.get_totp_auth_link()
        print("The response of TwoFactorAuthV1alpha1UcApi->get_totp_auth_link:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwoFactorAuthV1alpha1UcApi->get_totp_auth_link: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**TotpAuthLinkResponse**](TotpAuthLinkResponse.md)

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

# **get_two_factor_authentication_settings**
> TwoFactorAuthSettings get_two_factor_authentication_settings()

Get Two-factor authentication settings.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.two_factor_auth_settings import TwoFactorAuthSettings
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
    api_instance = halo_client.TwoFactorAuthV1alpha1UcApi(api_client)

    try:
        api_response = api_instance.get_two_factor_authentication_settings()
        print("The response of TwoFactorAuthV1alpha1UcApi->get_two_factor_authentication_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TwoFactorAuthV1alpha1UcApi->get_two_factor_authentication_settings: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**TwoFactorAuthSettings**](TwoFactorAuthSettings.md)

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

