# plesk_wp_toolkit_client.InstallationsFeaturesDebugApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_word_press_debug_settings**](InstallationsFeaturesDebugApi.md#get_word_press_debug_settings) | **GET** /v1/installations/{installationId}/features/debug/settings | 
[**update_word_press_debug_settings**](InstallationsFeaturesDebugApi.md#update_word_press_debug_settings) | **PATCH** /v1/installations/{installationId}/features/debug/settings | 
[**update_word_press_debug_status**](InstallationsFeaturesDebugApi.md#update_word_press_debug_status) | **PUT** /v1/installations/{installationId}/features/debug/status | 


# **get_word_press_debug_settings**
> WordPressDebugSettingsResponse get_word_press_debug_settings(installation_id)



Returns WordPress debug settings

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.word_press_debug_settings_response import WordPressDebugSettingsResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesDebugApi(api_client)
    installation_id = 1 # int | Installation ID

    try:
        api_response = api_instance.get_word_press_debug_settings(installation_id)
        print("The response of InstallationsFeaturesDebugApi->get_word_press_debug_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesDebugApi->get_word_press_debug_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 

### Return type

[**WordPressDebugSettingsResponse**](WordPressDebugSettingsResponse.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad Request |  -  |
**401** | Unauthorized |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_word_press_debug_settings**
> WordPressDebugSettingsResponse update_word_press_debug_settings(installation_id, word_press_debug_settings_request)



Update WordPress debug settings

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.word_press_debug_settings_request import WordPressDebugSettingsRequest
from plesk_wp_toolkit_client.models.word_press_debug_settings_response import WordPressDebugSettingsResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesDebugApi(api_client)
    installation_id = 1 # int | Installation ID
    word_press_debug_settings_request = plesk_wp_toolkit_client.WordPressDebugSettingsRequest() # WordPressDebugSettingsRequest | 

    try:
        api_response = api_instance.update_word_press_debug_settings(installation_id, word_press_debug_settings_request)
        print("The response of InstallationsFeaturesDebugApi->update_word_press_debug_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesDebugApi->update_word_press_debug_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **word_press_debug_settings_request** | [**WordPressDebugSettingsRequest**](WordPressDebugSettingsRequest.md)|  | 

### Return type

[**WordPressDebugSettingsResponse**](WordPressDebugSettingsResponse.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad Request |  -  |
**401** | Unauthorized |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_word_press_debug_status**
> WordPressDebugStatusResponse update_word_press_debug_status(installation_id, word_press_debug_status_request)



Update WordPress debug status

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.word_press_debug_status_request import WordPressDebugStatusRequest
from plesk_wp_toolkit_client.models.word_press_debug_status_response import WordPressDebugStatusResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesDebugApi(api_client)
    installation_id = 1 # int | Installation ID
    word_press_debug_status_request = plesk_wp_toolkit_client.WordPressDebugStatusRequest() # WordPressDebugStatusRequest | 

    try:
        api_response = api_instance.update_word_press_debug_status(installation_id, word_press_debug_status_request)
        print("The response of InstallationsFeaturesDebugApi->update_word_press_debug_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesDebugApi->update_word_press_debug_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **word_press_debug_status_request** | [**WordPressDebugStatusRequest**](WordPressDebugStatusRequest.md)|  | 

### Return type

[**WordPressDebugStatusResponse**](WordPressDebugStatusResponse.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | WordPress debug status |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

