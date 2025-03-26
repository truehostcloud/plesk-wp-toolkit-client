# plesk_wp_toolkit_client.InstallationsFeaturesCloneApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**clone_installation**](InstallationsFeaturesCloneApi.md#clone_installation) | **POST** /v1/cloner | 
[**get_clone_stub**](InstallationsFeaturesCloneApi.md#get_clone_stub) | **GET** /v1/installations/{installationId}/features/clone/stub | 
[**validate_clone_path**](InstallationsFeaturesCloneApi.md#validate_clone_path) | **POST** /v1/installations/{installationId}/features/clone/path-validator | 


# **clone_installation**
> BackgroundTaskWithUrlResponse clone_installation(installation_clone_request)



Clone WordPress installation

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.background_task_with_url_response import BackgroundTaskWithUrlResponse
from plesk_wp_toolkit_client.models.installation_clone_request import InstallationCloneRequest
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesCloneApi(api_client)
    installation_clone_request = plesk_wp_toolkit_client.InstallationCloneRequest() # InstallationCloneRequest | 

    try:
        api_response = api_instance.clone_installation(installation_clone_request)
        print("The response of InstallationsFeaturesCloneApi->clone_installation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesCloneApi->clone_installation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_clone_request** | [**InstallationCloneRequest**](InstallationCloneRequest.md)|  | 

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

# **get_clone_stub**
> CloneStubResponse get_clone_stub(installation_id, database_name=database_name, database_server=database_server, domain_existing=domain_existing, domain_new_subdomain_name=domain_new_subdomain_name, domain_new_subdomain_parent_domain=domain_new_subdomain_parent_domain, installation_path=installation_path)



Get default cloning options

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.clone_stub_response import CloneStubResponse
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesCloneApi(api_client)
    installation_id = 1 # int | Installation ID
    database_name = 'wp_im7zx' # str | Database name (optional)
    database_server = '1' # str | Database server ID (Plesk only) (optional)
    domain_existing = 'example.com' # str | Domain name (optional)
    domain_new_subdomain_name = 'staging' # str | Subdomain name (optional)
    domain_new_subdomain_parent_domain = 'example.com' # str | Domain name (optional)
    installation_path = 'wordpress-clone' # str | Installation path of cloned WordPress site (relative to the root directory of the domain) (optional)

    try:
        api_response = api_instance.get_clone_stub(installation_id, database_name=database_name, database_server=database_server, domain_existing=domain_existing, domain_new_subdomain_name=domain_new_subdomain_name, domain_new_subdomain_parent_domain=domain_new_subdomain_parent_domain, installation_path=installation_path)
        print("The response of InstallationsFeaturesCloneApi->get_clone_stub:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesCloneApi->get_clone_stub: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **database_name** | **str**| Database name | [optional] 
 **database_server** | **str**| Database server ID (Plesk only) | [optional] 
 **domain_existing** | **str**| Domain name | [optional] 
 **domain_new_subdomain_name** | **str**| Subdomain name | [optional] 
 **domain_new_subdomain_parent_domain** | **str**| Domain name | [optional] 
 **installation_path** | **str**| Installation path of cloned WordPress site (relative to the root directory of the domain) | [optional] 

### Return type

[**CloneStubResponse**](CloneStubResponse.md)

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

# **validate_clone_path**
> validate_clone_path(installation_id, clone_path_validator_request)



Validate installation path of a WordPress site clone on domain

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.clone_path_validator_request import ClonePathValidatorRequest
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesCloneApi(api_client)
    installation_id = 1 # int | Installation ID
    clone_path_validator_request = plesk_wp_toolkit_client.ClonePathValidatorRequest() # ClonePathValidatorRequest | 

    try:
        api_instance.validate_clone_path(installation_id, clone_path_validator_request)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesCloneApi->validate_clone_path: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installation_id** | **int**| Installation ID | 
 **clone_path_validator_request** | [**ClonePathValidatorRequest**](ClonePathValidatorRequest.md)|  | 

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
**422** | Unprocessable entity |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

