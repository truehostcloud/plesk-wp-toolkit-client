# plesk_wp_toolkit_client.InstallationsFeaturesHotlinkProtectionApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_hotlink_protection_settings_meta**](InstallationsFeaturesHotlinkProtectionApi.md#get_hotlink_protection_settings_meta) | **GET** /v1/installations/{installationId}/features/hotlink-protection/settings/meta | 
[**reset_hotlink_protection_settings**](InstallationsFeaturesHotlinkProtectionApi.md#reset_hotlink_protection_settings) | **DELETE** /v1/installations/{installationId}/features/hotlink-protection/settings | 
[**update_hotlink_protection_settings**](InstallationsFeaturesHotlinkProtectionApi.md#update_hotlink_protection_settings) | **PUT** /v1/installations/{installationId}/features/hotlink-protection/settings | 
[**update_hotlink_protection_status**](InstallationsFeaturesHotlinkProtectionApi.md#update_hotlink_protection_status) | **PUT** /v1/installations/{installationId}/features/hotlink-protection/status | 


# **get_hotlink_protection_settings_meta**
> MetaHotlinkProtectionSettings get_hotlink_protection_settings_meta(installation_id)



Get hotlink protection settings on a site

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.meta_hotlink_protection_settings import MetaHotlinkProtectionSettings
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesHotlinkProtectionApi(api_client)
    installation_id = 1 # int | Installation ID

    try:
        api_response = api_instance.get_hotlink_protection_settings_meta(installation_id)
        print("The response of InstallationsFeaturesHotlinkProtectionApi->get_hotlink_protection_settings_meta:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesHotlinkProtectionApi->get_hotlink_protection_settings_meta: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 

### Return type

[**MetaHotlinkProtectionSettings**](MetaHotlinkProtectionSettings.md)

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

# **reset_hotlink_protection_settings**
> HotlinkProtectionSettings reset_hotlink_protection_settings(installation_id, basic_delete_request=basic_delete_request)



Reset hotlink protection settings to default on a site

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.basic_delete_request import BasicDeleteRequest
from plesk_wp_toolkit_client.models.hotlink_protection_settings import HotlinkProtectionSettings
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesHotlinkProtectionApi(api_client)
    installation_id = 1 # int | Installation ID
    basic_delete_request = plesk_wp_toolkit_client.BasicDeleteRequest() # BasicDeleteRequest |  (optional)

    try:
        api_response = api_instance.reset_hotlink_protection_settings(installation_id, basic_delete_request=basic_delete_request)
        print("The response of InstallationsFeaturesHotlinkProtectionApi->reset_hotlink_protection_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesHotlinkProtectionApi->reset_hotlink_protection_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **basic_delete_request** | [**BasicDeleteRequest**](BasicDeleteRequest.md)|  | [optional] 

### Return type

[**HotlinkProtectionSettings**](HotlinkProtectionSettings.md)

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
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_hotlink_protection_settings**
> HotlinkProtectionSettings update_hotlink_protection_settings(installation_id, hotlink_protection_settings_request)



Update hotlink protection settings on a site

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.hotlink_protection_settings import HotlinkProtectionSettings
from plesk_wp_toolkit_client.models.hotlink_protection_settings_request import HotlinkProtectionSettingsRequest
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesHotlinkProtectionApi(api_client)
    installation_id = 1 # int | Installation ID
    hotlink_protection_settings_request = plesk_wp_toolkit_client.HotlinkProtectionSettingsRequest() # HotlinkProtectionSettingsRequest | 

    try:
        api_response = api_instance.update_hotlink_protection_settings(installation_id, hotlink_protection_settings_request)
        print("The response of InstallationsFeaturesHotlinkProtectionApi->update_hotlink_protection_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesHotlinkProtectionApi->update_hotlink_protection_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **hotlink_protection_settings_request** | [**HotlinkProtectionSettingsRequest**](HotlinkProtectionSettingsRequest.md)|  | 

### Return type

[**HotlinkProtectionSettings**](HotlinkProtectionSettings.md)

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
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_hotlink_protection_status**
> HotlinkProtectionStatusResponse update_hotlink_protection_status(installation_id, hotlink_protection_status_request)



Update hotlink protection status on a site

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.hotlink_protection_status_request import HotlinkProtectionStatusRequest
from plesk_wp_toolkit_client.models.hotlink_protection_status_response import HotlinkProtectionStatusResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesHotlinkProtectionApi(api_client)
    installation_id = 1 # int | Installation ID
    hotlink_protection_status_request = plesk_wp_toolkit_client.HotlinkProtectionStatusRequest() # HotlinkProtectionStatusRequest | 

    try:
        api_response = api_instance.update_hotlink_protection_status(installation_id, hotlink_protection_status_request)
        print("The response of InstallationsFeaturesHotlinkProtectionApi->update_hotlink_protection_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesHotlinkProtectionApi->update_hotlink_protection_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **hotlink_protection_status_request** | [**HotlinkProtectionStatusRequest**](HotlinkProtectionStatusRequest.md)|  | 

### Return type

[**HotlinkProtectionStatusResponse**](HotlinkProtectionStatusResponse.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Hotlink protection status on a site |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

