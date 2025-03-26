# plesk_wp_toolkit_client.InstallationsFeaturesMaintenanceApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_maintenance_preview**](InstallationsFeaturesMaintenanceApi.md#create_maintenance_preview) | **POST** /v1/installations/{installationId}/features/maintenance/preview | 
[**get_maintenance_settings**](InstallationsFeaturesMaintenanceApi.md#get_maintenance_settings) | **GET** /v1/installations/{installationId}/features/maintenance/settings | 
[**get_maintenance_template_customization_url**](InstallationsFeaturesMaintenanceApi.md#get_maintenance_template_customization_url) | **GET** /v1/installations/{installationId}/features/maintenance/template-customization-url | 
[**restore_maintenance_template**](InstallationsFeaturesMaintenanceApi.md#restore_maintenance_template) | **DELETE** /v1/installations/{installationId}/features/maintenance/template | 
[**update_maintenance_settings**](InstallationsFeaturesMaintenanceApi.md#update_maintenance_settings) | **PUT** /v1/installations/{installationId}/features/maintenance/settings | 
[**update_maintenance_status**](InstallationsFeaturesMaintenanceApi.md#update_maintenance_status) | **PUT** /v1/installations/{installationId}/features/maintenance/status | 


# **create_maintenance_preview**
> MaintenancePreviewResponse create_maintenance_preview(installation_id, maintenance_preview_request)



Create a preview of the maintenance mode page

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.maintenance_preview_request import MaintenancePreviewRequest
from plesk_wp_toolkit_client.models.maintenance_preview_response import MaintenancePreviewResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesMaintenanceApi(api_client)
    installation_id = 1 # int | Installation ID
    maintenance_preview_request = plesk_wp_toolkit_client.MaintenancePreviewRequest() # MaintenancePreviewRequest | 

    try:
        api_response = api_instance.create_maintenance_preview(installation_id, maintenance_preview_request)
        print("The response of InstallationsFeaturesMaintenanceApi->create_maintenance_preview:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesMaintenanceApi->create_maintenance_preview: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **maintenance_preview_request** | [**MaintenancePreviewRequest**](MaintenancePreviewRequest.md)|  | 

### Return type

[**MaintenancePreviewResponse**](MaintenancePreviewResponse.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_maintenance_settings**
> MaintenanceSettingsResponse get_maintenance_settings(installation_id)



Retrieve maintenance mode settings

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.maintenance_settings_response import MaintenanceSettingsResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesMaintenanceApi(api_client)
    installation_id = 1 # int | Installation ID

    try:
        api_response = api_instance.get_maintenance_settings(installation_id)
        print("The response of InstallationsFeaturesMaintenanceApi->get_maintenance_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesMaintenanceApi->get_maintenance_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 

### Return type

[**MaintenanceSettingsResponse**](MaintenanceSettingsResponse.md)

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

# **get_maintenance_template_customization_url**
> MaintenanceTemplateCustomizationUrlResponse get_maintenance_template_customization_url(installation_id)



Retrieve maintenance mode template URL

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.maintenance_template_customization_url_response import MaintenanceTemplateCustomizationUrlResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesMaintenanceApi(api_client)
    installation_id = 1 # int | Installation ID

    try:
        api_response = api_instance.get_maintenance_template_customization_url(installation_id)
        print("The response of InstallationsFeaturesMaintenanceApi->get_maintenance_template_customization_url:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesMaintenanceApi->get_maintenance_template_customization_url: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 

### Return type

[**MaintenanceTemplateCustomizationUrlResponse**](MaintenanceTemplateCustomizationUrlResponse.md)

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

# **restore_maintenance_template**
> restore_maintenance_template(installation_id, basic_delete_request=basic_delete_request)



Restore default maintenance mode template

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.basic_delete_request import BasicDeleteRequest
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesMaintenanceApi(api_client)
    installation_id = 1 # int | Installation ID
    basic_delete_request = plesk_wp_toolkit_client.BasicDeleteRequest() # BasicDeleteRequest |  (optional)

    try:
        api_instance.restore_maintenance_template(installation_id, basic_delete_request=basic_delete_request)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesMaintenanceApi->restore_maintenance_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **basic_delete_request** | [**BasicDeleteRequest**](BasicDeleteRequest.md)|  | [optional] 

### Return type

void (empty response body)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | No Content |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_maintenance_settings**
> MaintenanceSettingsResponse update_maintenance_settings(installation_id, maintenance_settings_request)



Update maintenance mode settings

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.maintenance_settings_request import MaintenanceSettingsRequest
from plesk_wp_toolkit_client.models.maintenance_settings_response import MaintenanceSettingsResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesMaintenanceApi(api_client)
    installation_id = 1 # int | Installation ID
    maintenance_settings_request = plesk_wp_toolkit_client.MaintenanceSettingsRequest() # MaintenanceSettingsRequest | 

    try:
        api_response = api_instance.update_maintenance_settings(installation_id, maintenance_settings_request)
        print("The response of InstallationsFeaturesMaintenanceApi->update_maintenance_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesMaintenanceApi->update_maintenance_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **maintenance_settings_request** | [**MaintenanceSettingsRequest**](MaintenanceSettingsRequest.md)|  | 

### Return type

[**MaintenanceSettingsResponse**](MaintenanceSettingsResponse.md)

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
**422** | Unprocessable entity |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_maintenance_status**
> StatusResponse update_maintenance_status(installation_id, status_request)



Toggle maintenance mode

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.status_request import StatusRequest
from plesk_wp_toolkit_client.models.status_response import StatusResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesMaintenanceApi(api_client)
    installation_id = 1 # int | Installation ID
    status_request = plesk_wp_toolkit_client.StatusRequest() # StatusRequest | 

    try:
        api_response = api_instance.update_maintenance_status(installation_id, status_request)
        print("The response of InstallationsFeaturesMaintenanceApi->update_maintenance_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesMaintenanceApi->update_maintenance_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **status_request** | [**StatusRequest**](StatusRequest.md)|  | 

### Return type

[**StatusResponse**](StatusResponse.md)

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

