# plesk_wp_toolkit_client.InstallationsThemesApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_installation_themes**](InstallationsThemesApi.md#get_installation_themes) | **GET** /v1/installations/{installationId}/themes | 
[**get_installations_themes**](InstallationsThemesApi.md#get_installations_themes) | **GET** /v1/installations/{installationId}/features/catalog/themes | 
[**instalations_themes_activate**](InstallationsThemesApi.md#instalations_themes_activate) | **PUT** /v1/installations/{installationId}/themes/{slug}/status | 
[**instalations_themes_install**](InstallationsThemesApi.md#instalations_themes_install) | **POST** /v1/installations/{installationId}/themes | 
[**instalations_themes_uninstall**](InstallationsThemesApi.md#instalations_themes_uninstall) | **DELETE** /v1/installations/{installationId}/themes | 
[**instalations_themes_upload_and_install**](InstallationsThemesApi.md#instalations_themes_upload_and_install) | **POST** /v1/installations/{installationId}/features/uploader/themes | 
[**update_installations_themes**](InstallationsThemesApi.md#update_installations_themes) | **PATCH** /v1/installations/{installationId}/themes | 


# **get_installation_themes**
> List[InstallationTheme] get_installation_themes(installation_id)



Get the list of themes on a WordPress installation

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.installation_theme import InstallationTheme
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
    api_instance = plesk_wp_toolkit_client.InstallationsThemesApi(api_client)
    installation_id = 1 # int | Installation ID

    try:
        api_response = api_instance.get_installation_themes(installation_id)
        print("The response of InstallationsThemesApi->get_installation_themes:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsThemesApi->get_installation_themes: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 

### Return type

[**List[InstallationTheme]**](InstallationTheme.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Installation theme list |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_installations_themes**
> WordPressAssetsCatalogResponse get_installations_themes(installation_id, page, page_size, compatible=compatible, download_count=download_count, last_updated_at=last_updated_at, rating=rating, term=term)



Get the list of themes for an installation

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
    api_instance = plesk_wp_toolkit_client.InstallationsThemesApi(api_client)
    installation_id = 56 # int | Installation ID
    page = 1 # int | Page number
    page_size = 25 # int | Items per page
    compatible = False # bool | Flag to output only compatible assets (optional) (default to False)
    download_count = 100000 # int | The minimum number of installations (optional)
    last_updated_at = all # str | Asset was updated later than current date minus a selected value (optional) (default to all)
    rating = 4.0 # float | The minimum rating of asset (optional)
    term = '' # str | Search term (optional) (default to '')

    try:
        api_response = api_instance.get_installations_themes(installation_id, page, page_size, compatible=compatible, download_count=download_count, last_updated_at=last_updated_at, rating=rating, term=term)
        print("The response of InstallationsThemesApi->get_installations_themes:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsThemesApi->get_installations_themes: %s\n" % e)
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

# **instalations_themes_activate**
> StatusResponse instalations_themes_activate(installation_id, slug, status_request)



Activate theme on a WordPress installation

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
    api_instance = plesk_wp_toolkit_client.InstallationsThemesApi(api_client)
    installation_id = 56 # int | Installation ID
    slug = 'slug_example' # str | Theme slug
    status_request = plesk_wp_toolkit_client.StatusRequest() # StatusRequest | 

    try:
        api_response = api_instance.instalations_themes_activate(installation_id, slug, status_request)
        print("The response of InstallationsThemesApi->instalations_themes_activate:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsThemesApi->instalations_themes_activate: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **slug** | **str**| Theme slug | 
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

# **instalations_themes_install**
> InstallationTheme instalations_themes_install(installation_id, installation_asset_install_request)



Install a theme on a WordPress installation

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.installation_asset_install_request import InstallationAssetInstallRequest
from plesk_wp_toolkit_client.models.installation_theme import InstallationTheme
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
    api_instance = plesk_wp_toolkit_client.InstallationsThemesApi(api_client)
    installation_id = 56 # int | Installation ID
    installation_asset_install_request = plesk_wp_toolkit_client.InstallationAssetInstallRequest() # InstallationAssetInstallRequest | 

    try:
        api_response = api_instance.instalations_themes_install(installation_id, installation_asset_install_request)
        print("The response of InstallationsThemesApi->instalations_themes_install:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsThemesApi->instalations_themes_install: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **installation_asset_install_request** | [**InstallationAssetInstallRequest**](InstallationAssetInstallRequest.md)|  | 

### Return type

[**InstallationTheme**](InstallationTheme.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Theme info |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **instalations_themes_uninstall**
> instalations_themes_uninstall(installation_id, request_body)



Uninstall themes from a WordPress installation

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
    api_instance = plesk_wp_toolkit_client.InstallationsThemesApi(api_client)
    installation_id = 56 # int | Installation ID
    request_body = ['hello-dolly', 'twentytwenty'] # List[str] | 

    try:
        api_instance.instalations_themes_uninstall(installation_id, request_body)
    except Exception as e:
        print("Exception when calling InstallationsThemesApi->instalations_themes_uninstall: %s\n" % e)
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

# **instalations_themes_upload_and_install**
> BackgroundTaskWithUrlResponse instalations_themes_upload_and_install(installation_id, file, status)



Upload and install a theme on a WordPress installation

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
    api_instance = plesk_wp_toolkit_client.InstallationsThemesApi(api_client)
    installation_id = 56 # int | Installation ID
    file = None # bytearray | File name
    status = True # bool | Activate or not the asset after upload

    try:
        api_response = api_instance.instalations_themes_upload_and_install(installation_id, file, status)
        print("The response of InstallationsThemesApi->instalations_themes_upload_and_install:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsThemesApi->instalations_themes_upload_and_install: %s\n" % e)
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

# **update_installations_themes**
> List[InstallationTheme] update_installations_themes(installation_id, installation_asset_update_request)



Change auto updates setting for themes on a WordPress installation

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.installation_asset_update_request import InstallationAssetUpdateRequest
from plesk_wp_toolkit_client.models.installation_theme import InstallationTheme
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
    api_instance = plesk_wp_toolkit_client.InstallationsThemesApi(api_client)
    installation_id = 56 # int | Installation ID
    installation_asset_update_request = [plesk_wp_toolkit_client.InstallationAssetUpdateRequest()] # List[InstallationAssetUpdateRequest] | 

    try:
        api_response = api_instance.update_installations_themes(installation_id, installation_asset_update_request)
        print("The response of InstallationsThemesApi->update_installations_themes:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsThemesApi->update_installations_themes: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **installation_asset_update_request** | [**List[InstallationAssetUpdateRequest]**](InstallationAssetUpdateRequest.md)|  | 

### Return type

[**List[InstallationTheme]**](InstallationTheme.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Installation theme list |  -  |
**400** | Bad Request |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

