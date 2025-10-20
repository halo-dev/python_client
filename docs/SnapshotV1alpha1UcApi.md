# halo_client.SnapshotV1alpha1UcApi

All URIs are relative to *http://localhost:8091*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_snapshot_for_post**](SnapshotV1alpha1UcApi.md#get_snapshot_for_post) | **GET** /apis/uc.api.content.halo.run/v1alpha1/snapshots/{name} | 


# **get_snapshot_for_post**
> Snapshot get_snapshot_for_post(name, post_name, patched=patched)

Get snapshot for one post.

### Example

* Basic Authentication (basicAuth):
* Bearer (JWT) Authentication (bearerAuth):

```python
import halo_client
from halo_client.models.snapshot import Snapshot
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
    api_instance = halo_client.SnapshotV1alpha1UcApi(api_client)
    name = 'name_example' # str | Snapshot name.
    post_name = 'post_name_example' # str | Post name.
    patched = True # bool | Should include patched content and raw or not. (optional)

    try:
        api_response = api_instance.get_snapshot_for_post(name, post_name, patched=patched)
        print("The response of SnapshotV1alpha1UcApi->get_snapshot_for_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SnapshotV1alpha1UcApi->get_snapshot_for_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Snapshot name. | 
 **post_name** | **str**| Post name. | 
 **patched** | **bool**| Should include patched content and raw or not. | [optional] 

### Return type

[**Snapshot**](Snapshot.md)

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

