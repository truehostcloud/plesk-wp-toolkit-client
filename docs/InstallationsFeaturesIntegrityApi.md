# plesk_wp_toolkit_client.InstallationsFeaturesIntegrityApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_integrity**](InstallationsFeaturesIntegrityApi.md#get_integrity) | **GET** /v1/installations/{installationId}/features/integrity | 


# **get_integrity**
> Integrity get_integrity(installation_id)



Get information about WordPress integrity check

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.integrity import Integrity
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesIntegrityApi(api_client)
    installation_id = 1 # int | Installation ID

    try:
        api_response = api_instance.get_integrity(installation_id)
        print("The response of InstallationsFeaturesIntegrityApi->get_integrity:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesIntegrityApi->get_integrity: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 

### Return type

[**Integrity**](Integrity.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Information about WordPress integrity check |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

