# plesk_wp_toolkit_client.InstallationsFeaturesUpdatesApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_auto_update_settings**](InstallationsFeaturesUpdatesApi.md#get_auto_update_settings) | **GET** /v1/installations/{installationId}/features/updates/settings | 
[**update_auto_update_settings**](InstallationsFeaturesUpdatesApi.md#update_auto_update_settings) | **PUT** /v1/installations/{installationId}/features/updates/settings | 
[**update_installations_auto_updates_settings**](InstallationsFeaturesUpdatesApi.md#update_installations_auto_updates_settings) | **POST** /v1/features/updates/settings | 
[**update_installations_auto_updates_settings_v2**](InstallationsFeaturesUpdatesApi.md#update_installations_auto_updates_settings_v2) | **POST** /v2/features/updates/settings | 


# **get_auto_update_settings**
> InstallationAutoUpdateResponse get_auto_update_settings(installation_id)



Get autoupdate settings

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.installation_auto_update_response import InstallationAutoUpdateResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesUpdatesApi(api_client)
    installation_id = 1 # int | Installation ID

    try:
        api_response = api_instance.get_auto_update_settings(installation_id)
        print("The response of InstallationsFeaturesUpdatesApi->get_auto_update_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesUpdatesApi->get_auto_update_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 

### Return type

[**InstallationAutoUpdateResponse**](InstallationAutoUpdateResponse.md)

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

# **update_auto_update_settings**
> InstallationAutoUpdateResponse update_auto_update_settings(installation_id, installation_auto_update_request)



Change autoupdate settings

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.installation_auto_update_request import InstallationAutoUpdateRequest
from plesk_wp_toolkit_client.models.installation_auto_update_response import InstallationAutoUpdateResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesUpdatesApi(api_client)
    installation_id = 1 # int | Installation ID
    installation_auto_update_request = plesk_wp_toolkit_client.InstallationAutoUpdateRequest() # InstallationAutoUpdateRequest | 

    try:
        api_response = api_instance.update_auto_update_settings(installation_id, installation_auto_update_request)
        print("The response of InstallationsFeaturesUpdatesApi->update_auto_update_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesUpdatesApi->update_auto_update_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **installation_auto_update_request** | [**InstallationAutoUpdateRequest**](InstallationAutoUpdateRequest.md)|  | 

### Return type

[**InstallationAutoUpdateResponse**](InstallationAutoUpdateResponse.md)

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

# **update_installations_auto_updates_settings**
> List[InstallationAutoUpdateWithIdResponse] update_installations_auto_updates_settings(installations_auto_update_request, skip_broken_installations=skip_broken_installations, skip_infected_installations=skip_infected_installations, skip_unsupported_installations=skip_unsupported_installations)



Change autoupdate settings

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.installation_auto_update_with_id_response import InstallationAutoUpdateWithIdResponse
from plesk_wp_toolkit_client.models.installations_auto_update_request import InstallationsAutoUpdateRequest
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesUpdatesApi(api_client)
    installations_auto_update_request = plesk_wp_toolkit_client.InstallationsAutoUpdateRequest() # InstallationsAutoUpdateRequest | 
    skip_broken_installations = false # bool | Ignore broken installations (by default request fails on them) (optional)
    skip_infected_installations = false # bool | Ignore quarantined installations (by default request fails on them) (optional)
    skip_unsupported_installations = false # bool | Ignore unsupported installations (by default request fails on them) (optional)

    try:
        api_response = api_instance.update_installations_auto_updates_settings(installations_auto_update_request, skip_broken_installations=skip_broken_installations, skip_infected_installations=skip_infected_installations, skip_unsupported_installations=skip_unsupported_installations)
        print("The response of InstallationsFeaturesUpdatesApi->update_installations_auto_updates_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesUpdatesApi->update_installations_auto_updates_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installations_auto_update_request** | [**InstallationsAutoUpdateRequest**](InstallationsAutoUpdateRequest.md)|  | 
 **skip_broken_installations** | **bool**| Ignore broken installations (by default request fails on them) | [optional] 
 **skip_infected_installations** | **bool**| Ignore quarantined installations (by default request fails on them) | [optional] 
 **skip_unsupported_installations** | **bool**| Ignore unsupported installations (by default request fails on them) | [optional] 

### Return type

[**List[InstallationAutoUpdateWithIdResponse]**](InstallationAutoUpdateWithIdResponse.md)

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
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_installations_auto_updates_settings_v2**
> BackgroundTaskWithUrlResponse update_installations_auto_updates_settings_v2(installations_auto_update_request, skip_broken_installations=skip_broken_installations, skip_infected_installations=skip_infected_installations, skip_unsupported_installations=skip_unsupported_installations)



Change autoupdate settings

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.background_task_with_url_response import BackgroundTaskWithUrlResponse
from plesk_wp_toolkit_client.models.installations_auto_update_request import InstallationsAutoUpdateRequest
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesUpdatesApi(api_client)
    installations_auto_update_request = plesk_wp_toolkit_client.InstallationsAutoUpdateRequest() # InstallationsAutoUpdateRequest | 
    skip_broken_installations = false # bool | Ignore broken installations (by default request fails on them) (optional)
    skip_infected_installations = false # bool | Ignore quarantined installations (by default request fails on them) (optional)
    skip_unsupported_installations = false # bool | Ignore unsupported installations (by default request fails on them) (optional)

    try:
        api_response = api_instance.update_installations_auto_updates_settings_v2(installations_auto_update_request, skip_broken_installations=skip_broken_installations, skip_infected_installations=skip_infected_installations, skip_unsupported_installations=skip_unsupported_installations)
        print("The response of InstallationsFeaturesUpdatesApi->update_installations_auto_updates_settings_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesUpdatesApi->update_installations_auto_updates_settings_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installations_auto_update_request** | [**InstallationsAutoUpdateRequest**](InstallationsAutoUpdateRequest.md)|  | 
 **skip_broken_installations** | **bool**| Ignore broken installations (by default request fails on them) | [optional] 
 **skip_infected_installations** | **bool**| Ignore quarantined installations (by default request fails on them) | [optional] 
 **skip_unsupported_installations** | **bool**| Ignore unsupported installations (by default request fails on them) | [optional] 

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
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

