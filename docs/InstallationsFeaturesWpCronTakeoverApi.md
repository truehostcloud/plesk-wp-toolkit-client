# plesk_wp_toolkit_client.InstallationsFeaturesWpCronTakeoverApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_wp_cron_takeover_meta**](InstallationsFeaturesWpCronTakeoverApi.md#get_wp_cron_takeover_meta) | **GET** /v1/installations/{installationId}/features/wp-cron-takeover/meta | 
[**update_wp_cron_takeover**](InstallationsFeaturesWpCronTakeoverApi.md#update_wp_cron_takeover) | **PATCH** /v1/installations/{installationId}/features/wp-cron-takeover | 


# **get_wp_cron_takeover_meta**
> MetaWpCronTakeoverInstanceFeature get_wp_cron_takeover_meta(installation_id)



Get status of wp-cron-takeover feature

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.meta_wp_cron_takeover_instance_feature import MetaWpCronTakeoverInstanceFeature
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesWpCronTakeoverApi(api_client)
    installation_id = 1 # int | Installation ID

    try:
        api_response = api_instance.get_wp_cron_takeover_meta(installation_id)
        print("The response of InstallationsFeaturesWpCronTakeoverApi->get_wp_cron_takeover_meta:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesWpCronTakeoverApi->get_wp_cron_takeover_meta: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 

### Return type

[**MetaWpCronTakeoverInstanceFeature**](MetaWpCronTakeoverInstanceFeature.md)

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
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_wp_cron_takeover**
> WpCronTakeoverInstanceFeature update_wp_cron_takeover(installation_id, wp_cron_takeover_instance_request)



Update wp-cron-takeover feature

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.wp_cron_takeover_instance_feature import WpCronTakeoverInstanceFeature
from plesk_wp_toolkit_client.models.wp_cron_takeover_instance_request import WpCronTakeoverInstanceRequest
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesWpCronTakeoverApi(api_client)
    installation_id = 1 # int | Installation ID
    wp_cron_takeover_instance_request = plesk_wp_toolkit_client.WpCronTakeoverInstanceRequest() # WpCronTakeoverInstanceRequest | 

    try:
        api_response = api_instance.update_wp_cron_takeover(installation_id, wp_cron_takeover_instance_request)
        print("The response of InstallationsFeaturesWpCronTakeoverApi->update_wp_cron_takeover:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesWpCronTakeoverApi->update_wp_cron_takeover: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **wp_cron_takeover_instance_request** | [**WpCronTakeoverInstanceRequest**](WpCronTakeoverInstanceRequest.md)|  | 

### Return type

[**WpCronTakeoverInstanceFeature**](WpCronTakeoverInstanceFeature.md)

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
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

