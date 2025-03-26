# plesk_wp_toolkit_client.SecurityMeasuresApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**check_security**](SecurityMeasuresApi.md#check_security) | **POST** /v1/security-measures/checker | 
[**get_security_measures**](SecurityMeasuresApi.md#get_security_measures) | **GET** /v1/security-measures | 
[**get_security_measures_per_installations**](SecurityMeasuresApi.md#get_security_measures_per_installations) | **GET** /v1/security-measures/checker | 
[**resolve_security_measures**](SecurityMeasuresApi.md#resolve_security_measures) | **POST** /v1/security-measures/resolver | 
[**revert_security_measures**](SecurityMeasuresApi.md#revert_security_measures) | **POST** /v1/security-measures/reverter | 


# **check_security**
> BackgroundTaskWithUrlResponse check_security(security_measures_check_security_request)



Check security measure status

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.background_task_with_url_response import BackgroundTaskWithUrlResponse
from plesk_wp_toolkit_client.models.security_measures_check_security_request import SecurityMeasuresCheckSecurityRequest
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
    api_instance = plesk_wp_toolkit_client.SecurityMeasuresApi(api_client)
    security_measures_check_security_request = plesk_wp_toolkit_client.SecurityMeasuresCheckSecurityRequest() # SecurityMeasuresCheckSecurityRequest | 

    try:
        api_response = api_instance.check_security(security_measures_check_security_request)
        print("The response of SecurityMeasuresApi->check_security:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SecurityMeasuresApi->check_security: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **security_measures_check_security_request** | [**SecurityMeasuresCheckSecurityRequest**](SecurityMeasuresCheckSecurityRequest.md)|  | 

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_security_measures**
> List[SecurityMeasure] get_security_measures()



List available security measures

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.security_measure import SecurityMeasure
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
    api_instance = plesk_wp_toolkit_client.SecurityMeasuresApi(api_client)

    try:
        api_response = api_instance.get_security_measures()
        print("The response of SecurityMeasuresApi->get_security_measures:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SecurityMeasuresApi->get_security_measures: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[SecurityMeasure]**](SecurityMeasure.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Security measure list |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_security_measures_per_installations**
> List[SecurityMeasuresInstallationStatus] get_security_measures_per_installations(installations_ids=installations_ids, skip_broken_installations=skip_broken_installations, skip_infected_installations=skip_infected_installations, skip_unsupported_installations=skip_unsupported_installations)



List security measure status on installations

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.security_measures_installation_status import SecurityMeasuresInstallationStatus
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
    api_instance = plesk_wp_toolkit_client.SecurityMeasuresApi(api_client)
    installations_ids = [[1,3,5]] # List[int] | Array with installation IDs for filter (optional)
    skip_broken_installations = false # bool | Ignore broken installations (by default request fails on them) (optional)
    skip_infected_installations = false # bool | Ignore quarantined installations (by default request fails on them) (optional)
    skip_unsupported_installations = false # bool | Ignore unsupported installations (by default request fails on them) (optional)

    try:
        api_response = api_instance.get_security_measures_per_installations(installations_ids=installations_ids, skip_broken_installations=skip_broken_installations, skip_infected_installations=skip_infected_installations, skip_unsupported_installations=skip_unsupported_installations)
        print("The response of SecurityMeasuresApi->get_security_measures_per_installations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SecurityMeasuresApi->get_security_measures_per_installations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installations_ids** | [**List[int]**](int.md)| Array with installation IDs for filter | [optional] 
 **skip_broken_installations** | **bool**| Ignore broken installations (by default request fails on them) | [optional] 
 **skip_infected_installations** | **bool**| Ignore quarantined installations (by default request fails on them) | [optional] 
 **skip_unsupported_installations** | **bool**| Ignore unsupported installations (by default request fails on them) | [optional] 

### Return type

[**List[SecurityMeasuresInstallationStatus]**](SecurityMeasuresInstallationStatus.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Status of security measures |  -  |
**400** | Bad Request |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **resolve_security_measures**
> BackgroundTaskWithUrlResponse resolve_security_measures(security_measures_resolve_request)



Apply security measures

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.background_task_with_url_response import BackgroundTaskWithUrlResponse
from plesk_wp_toolkit_client.models.security_measures_resolve_request import SecurityMeasuresResolveRequest
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
    api_instance = plesk_wp_toolkit_client.SecurityMeasuresApi(api_client)
    security_measures_resolve_request = plesk_wp_toolkit_client.SecurityMeasuresResolveRequest() # SecurityMeasuresResolveRequest | 

    try:
        api_response = api_instance.resolve_security_measures(security_measures_resolve_request)
        print("The response of SecurityMeasuresApi->resolve_security_measures:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SecurityMeasuresApi->resolve_security_measures: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **security_measures_resolve_request** | [**SecurityMeasuresResolveRequest**](SecurityMeasuresResolveRequest.md)|  | 

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **revert_security_measures**
> BackgroundTaskWithUrlResponse revert_security_measures(security_measures_revert_request)



Revert security measures

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.background_task_with_url_response import BackgroundTaskWithUrlResponse
from plesk_wp_toolkit_client.models.security_measures_revert_request import SecurityMeasuresRevertRequest
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
    api_instance = plesk_wp_toolkit_client.SecurityMeasuresApi(api_client)
    security_measures_revert_request = plesk_wp_toolkit_client.SecurityMeasuresRevertRequest() # SecurityMeasuresRevertRequest | 

    try:
        api_response = api_instance.revert_security_measures(security_measures_revert_request)
        print("The response of SecurityMeasuresApi->revert_security_measures:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SecurityMeasuresApi->revert_security_measures: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **security_measures_revert_request** | [**SecurityMeasuresRevertRequest**](SecurityMeasuresRevertRequest.md)|  | 

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

