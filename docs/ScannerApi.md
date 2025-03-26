# plesk_wp_toolkit_client.ScannerApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**scan_installations**](ScannerApi.md#scan_installations) | **POST** /v1/scanner | 


# **scan_installations**
> BackgroundTaskWithUrlResponse scan_installations(basic_confirmation_request)



Scan WordPress installations

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.background_task_with_url_response import BackgroundTaskWithUrlResponse
from plesk_wp_toolkit_client.models.basic_confirmation_request import BasicConfirmationRequest
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
    api_instance = plesk_wp_toolkit_client.ScannerApi(api_client)
    basic_confirmation_request = plesk_wp_toolkit_client.BasicConfirmationRequest() # BasicConfirmationRequest | 

    try:
        api_response = api_instance.scan_installations(basic_confirmation_request)
        print("The response of ScannerApi->scan_installations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ScannerApi->scan_installations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **basic_confirmation_request** | [**BasicConfirmationRequest**](BasicConfirmationRequest.md)|  | 

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
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

