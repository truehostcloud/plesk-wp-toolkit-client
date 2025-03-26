# plesk_wp_toolkit_client.InstallationsPluginsApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_installation_plugins**](InstallationsPluginsApi.md#get_installation_plugins) | **GET** /v1/installations/{installationId}/plugins | 
[**get_installations_plugins**](InstallationsPluginsApi.md#get_installations_plugins) | **GET** /v1/installations/{installationId}/features/catalog/plugins | 
[**instalations_plugins_activate_deactivate**](InstallationsPluginsApi.md#instalations_plugins_activate_deactivate) | **PUT** /v1/installations/{installationId}/plugins/{slug}/status | 
[**instalations_plugins_info**](InstallationsPluginsApi.md#instalations_plugins_info) | **GET** /v1/installations/{installationId}/features/catalog/plugins/{slug} | 
[**instalations_plugins_install**](InstallationsPluginsApi.md#instalations_plugins_install) | **POST** /v1/installations/{installationId}/plugins | 
[**instalations_plugins_uninstall**](InstallationsPluginsApi.md#instalations_plugins_uninstall) | **DELETE** /v1/installations/{installationId}/plugins | 
[**instalations_plugins_upload_and_install**](InstallationsPluginsApi.md#instalations_plugins_upload_and_install) | **POST** /v1/installations/{installationId}/features/uploader/plugins | 
[**update_installations_plugins**](InstallationsPluginsApi.md#update_installations_plugins) | **PATCH** /v1/installations/{installationId}/plugins | 


# **get_installation_plugins**
> List[InstallationPlugin] get_installation_plugins(installation_id)



Get the list of plugins on a WordPress installation

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.installation_plugin import InstallationPlugin
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
    api_instance = plesk_wp_toolkit_client.InstallationsPluginsApi(api_client)
    installation_id = 1 # int | Installation ID

    try:
        api_response = api_instance.get_installation_plugins(installation_id)
        print("The response of InstallationsPluginsApi->get_installation_plugins:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsPluginsApi->get_installation_plugins: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 

### Return type

[**List[InstallationPlugin]**](InstallationPlugin.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Installation plugin list |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_installations_plugins**
> WordPressAssetsCatalogResponse get_installations_plugins(installation_id, page, page_size, compatible=compatible, download_count=download_count, last_updated_at=last_updated_at, rating=rating, term=term)



Get the list of plugins for an installation

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.word_press_assets_catalog_response import WordPressAssetsCatalogResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsPluginsApi(api_client)
    installation_id = 56 # int | Installation ID
    page = 1 # int | Page number
    page_size = 25 # int | Items per page
    compatible = False # bool | Flag to output only compatible assets (optional) (default to False)
    download_count = 100000 # int | The minimum number of installations (optional)
    last_updated_at = all # str | Asset was updated later than current date minus a selected value (optional) (default to all)
    rating = 4.0 # float | The minimum rating of asset (optional)
    term = '' # str | Search term (optional) (default to '')

    try:
        api_response = api_instance.get_installations_plugins(installation_id, page, page_size, compatible=compatible, download_count=download_count, last_updated_at=last_updated_at, rating=rating, term=term)
        print("The response of InstallationsPluginsApi->get_installations_plugins:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsPluginsApi->get_installations_plugins: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **page** | **int**| Page number | 
 **page_size** | **int**| Items per page | 
 **compatible** | **bool**| Flag to output only compatible assets | [optional] [default to False]
 **download_count** | **int**| The minimum number of installations | [optional] 
 **last_updated_at** | **str**| Asset was updated later than current date minus a selected value | [optional] [default to all]
 **rating** | **float**| The minimum rating of asset | [optional] 
 **term** | **str**| Search term | [optional] [default to &#39;&#39;]

### Return type

[**WordPressAssetsCatalogResponse**](WordPressAssetsCatalogResponse.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | WordPress available assets info |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **instalations_plugins_activate_deactivate**
> StatusResponse instalations_plugins_activate_deactivate(installation_id, slug, status_request)



Activate or deactivate plugin on a WordPress installation

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
    api_instance = plesk_wp_toolkit_client.InstallationsPluginsApi(api_client)
    installation_id = 56 # int | Installation ID
    slug = 'slug_example' # str | Plugin slug
    status_request = plesk_wp_toolkit_client.StatusRequest() # StatusRequest | 

    try:
        api_response = api_instance.instalations_plugins_activate_deactivate(installation_id, slug, status_request)
        print("The response of InstallationsPluginsApi->instalations_plugins_activate_deactivate:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsPluginsApi->instalations_plugins_activate_deactivate: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **slug** | **str**| Plugin slug | 
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

# **instalations_plugins_info**
> WordPressAsset instalations_plugins_info(installation_id, slug)



Retrieve plugin info from WordPress.org

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.word_press_asset import WordPressAsset
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
    api_instance = plesk_wp_toolkit_client.InstallationsPluginsApi(api_client)
    installation_id = 56 # int | Installation ID
    slug = 'slug_example' # str | Plugin slug

    try:
        api_response = api_instance.instalations_plugins_info(installation_id, slug)
        print("The response of InstallationsPluginsApi->instalations_plugins_info:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsPluginsApi->instalations_plugins_info: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **slug** | **str**| Plugin slug | 

### Return type

[**WordPressAsset**](WordPressAsset.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | WordPress asset info |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **instalations_plugins_install**
> InstallationPlugin instalations_plugins_install(installation_id, installation_asset_install_request)



Install a plugin on a WordPress installation

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.installation_asset_install_request import InstallationAssetInstallRequest
from plesk_wp_toolkit_client.models.installation_plugin import InstallationPlugin
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
    api_instance = plesk_wp_toolkit_client.InstallationsPluginsApi(api_client)
    installation_id = 56 # int | Installation ID
    installation_asset_install_request = plesk_wp_toolkit_client.InstallationAssetInstallRequest() # InstallationAssetInstallRequest | 

    try:
        api_response = api_instance.instalations_plugins_install(installation_id, installation_asset_install_request)
        print("The response of InstallationsPluginsApi->instalations_plugins_install:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsPluginsApi->instalations_plugins_install: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **installation_asset_install_request** | [**InstallationAssetInstallRequest**](InstallationAssetInstallRequest.md)|  | 

### Return type

[**InstallationPlugin**](InstallationPlugin.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Plugin info |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **instalations_plugins_uninstall**
> instalations_plugins_uninstall(installation_id, request_body)



Uninstall plugins from a WordPress installation

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
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
    api_instance = plesk_wp_toolkit_client.InstallationsPluginsApi(api_client)
    installation_id = 56 # int | Installation ID
    request_body = ['jetpack', 'akismet'] # List[str] | 

    try:
        api_instance.instalations_plugins_uninstall(installation_id, request_body)
    except Exception as e:
        print("Exception when calling InstallationsPluginsApi->instalations_plugins_uninstall: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **request_body** | [**List[str]**](str.md)|  | 

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

# **instalations_plugins_upload_and_install**
> BackgroundTaskWithUrlResponse instalations_plugins_upload_and_install(installation_id, file, status)



Upload and install a plugin on a WordPress installation

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.background_task_with_url_response import BackgroundTaskWithUrlResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsPluginsApi(api_client)
    installation_id = 56 # int | Installation ID
    file = None # bytearray | File name
    status = True # bool | Activate or not the asset after upload

    try:
        api_response = api_instance.instalations_plugins_upload_and_install(installation_id, file, status)
        print("The response of InstallationsPluginsApi->instalations_plugins_upload_and_install:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsPluginsApi->instalations_plugins_upload_and_install: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **file** | **bytearray**| File name | 
 **status** | **bool**| Activate or not the asset after upload | 

### Return type

[**BackgroundTaskWithUrlResponse**](BackgroundTaskWithUrlResponse.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | OK |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**422** | Unprocessable entity |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_installations_plugins**
> List[InstallationPlugin] update_installations_plugins(installation_id, installation_asset_update_request)



Change auto updates setting and/or status for plugins on a WordPress installation

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.installation_asset_update_request import InstallationAssetUpdateRequest
from plesk_wp_toolkit_client.models.installation_plugin import InstallationPlugin
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
    api_instance = plesk_wp_toolkit_client.InstallationsPluginsApi(api_client)
    installation_id = 56 # int | Installation ID
    installation_asset_update_request = [plesk_wp_toolkit_client.InstallationAssetUpdateRequest()] # List[InstallationAssetUpdateRequest] | 

    try:
        api_response = api_instance.update_installations_plugins(installation_id, installation_asset_update_request)
        print("The response of InstallationsPluginsApi->update_installations_plugins:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsPluginsApi->update_installations_plugins: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **installation_asset_update_request** | [**List[InstallationAssetUpdateRequest]**](InstallationAssetUpdateRequest.md)|  | 

### Return type

[**List[InstallationPlugin]**](InstallationPlugin.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Installation plugin list |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

