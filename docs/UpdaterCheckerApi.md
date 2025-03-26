# plesk_wp_toolkit_client.UpdaterCheckerApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_available_updates**](UpdaterCheckerApi.md#fetch_available_updates) | **GET** /v1/updates-checker | 
[**refresh_available_updates**](UpdaterCheckerApi.md#refresh_available_updates) | **POST** /v1/updates-checker | 


# **fetch_available_updates**
> List[WordPressUpdatesResponse] fetch_available_updates(installations_ids=installations_ids, skip_broken_installations=skip_broken_installations, skip_infected_installations=skip_infected_installations, skip_unsupported_installations=skip_unsupported_installations)



Get information about available updates

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.word_press_updates_response import WordPressUpdatesResponse
from plesk_wp_toolkit_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://example.com/api/modules/wp-toolkit
# See configuration.py for a list of all supported configuration parameters.
configuration = plesk_wp_toolkit_client.Configuration(
    host = "https://example.com/api/modules/wp-toolkit"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: httpBasic
configuration = plesk_wp_toolkit_client.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Configure API key authorization: pleskApiToken
configuration.api_key['pleskApiToken'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['pleskApiToken'] = 'Bearer'

# Enter a context with an instance of the API client
with plesk_wp_toolkit_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = plesk_wp_toolkit_client.UpdaterCheckerApi(api_client)
    installations_ids = [[1,3,5]] # List[int] | Array with installation IDs for filter (optional)
    skip_broken_installations = false # bool | Ignore broken installations (by default request fails on them) (optional)
    skip_infected_installations = false # bool | Ignore quarantined installations (by default request fails on them) (optional)
    skip_unsupported_installations = false # bool | Ignore unsupported installations (by default request fails on them) (optional)

    try:
        api_response = api_instance.fetch_available_updates(installations_ids=installations_ids, skip_broken_installations=skip_broken_installations, skip_infected_installations=skip_infected_installations, skip_unsupported_installations=skip_unsupported_installations)
        print("The response of UpdaterCheckerApi->fetch_available_updates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UpdaterCheckerApi->fetch_available_updates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installations_ids** | [**List[int]**](int.md)| Array with installation IDs for filter | [optional] 
 **skip_broken_installations** | **bool**| Ignore broken installations (by default request fails on them) | [optional] 
 **skip_infected_installations** | **bool**| Ignore quarantined installations (by default request fails on them) | [optional] 
 **skip_unsupported_installations** | **bool**| Ignore unsupported installations (by default request fails on them) | [optional] 

### Return type

[**List[WordPressUpdatesResponse]**](WordPressUpdatesResponse.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Available updates |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **refresh_available_updates**
> BackgroundTaskWithUrlResponse refresh_available_updates(refresh_available_updates_request=refresh_available_updates_request)



Start updates availability check

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.background_task_with_url_response import BackgroundTaskWithUrlResponse
from plesk_wp_toolkit_client.models.refresh_available_updates_request import RefreshAvailableUpdatesRequest
from plesk_wp_toolkit_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://example.com/api/modules/wp-toolkit
# See configuration.py for a list of all supported configuration parameters.
configuration = plesk_wp_toolkit_client.Configuration(
    host = "https://example.com/api/modules/wp-toolkit"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: httpBasic
configuration = plesk_wp_toolkit_client.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Configure API key authorization: pleskApiToken
configuration.api_key['pleskApiToken'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['pleskApiToken'] = 'Bearer'

# Enter a context with an instance of the API client
with plesk_wp_toolkit_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = plesk_wp_toolkit_client.UpdaterCheckerApi(api_client)
    refresh_available_updates_request = plesk_wp_toolkit_client.RefreshAvailableUpdatesRequest() # RefreshAvailableUpdatesRequest |  (optional)

    try:
        api_response = api_instance.refresh_available_updates(refresh_available_updates_request=refresh_available_updates_request)
        print("The response of UpdaterCheckerApi->refresh_available_updates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UpdaterCheckerApi->refresh_available_updates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **refresh_available_updates_request** | [**RefreshAvailableUpdatesRequest**](RefreshAvailableUpdatesRequest.md)|  | [optional] 

### Return type

[**BackgroundTaskWithUrlResponse**](BackgroundTaskWithUrlResponse.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | OK |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

