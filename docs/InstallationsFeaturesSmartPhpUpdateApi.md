# plesk_wp_toolkit_client.InstallationsFeaturesSmartPhpUpdateApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**run_smart_php_update**](InstallationsFeaturesSmartPhpUpdateApi.md#run_smart_php_update) | **POST** /v1/smart-php-updater | 


# **run_smart_php_update**
> BackgroundTaskWithUrlResponse run_smart_php_update(run_smart_php_update_request)



Run Smart PHP Update

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.background_task_with_url_response import BackgroundTaskWithUrlResponse
from plesk_wp_toolkit_client.models.run_smart_php_update_request import RunSmartPhpUpdateRequest
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesSmartPhpUpdateApi(api_client)
    run_smart_php_update_request = plesk_wp_toolkit_client.RunSmartPhpUpdateRequest() # RunSmartPhpUpdateRequest | 

    try:
        api_response = api_instance.run_smart_php_update(run_smart_php_update_request)
        print("The response of InstallationsFeaturesSmartPhpUpdateApi->run_smart_php_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesSmartPhpUpdateApi->run_smart_php_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **run_smart_php_update_request** | [**RunSmartPhpUpdateRequest**](RunSmartPhpUpdateRequest.md)|  | 

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
**401** | Unauthorized |  -  |
**404** | Not Found |  -  |
**422** | Unprocessable entity |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

