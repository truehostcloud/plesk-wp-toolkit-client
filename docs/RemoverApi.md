# plesk_wp_toolkit_client.RemoverApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_installations_remove_confirmation**](RemoverApi.md#get_installations_remove_confirmation) | **GET** /v1/remover/confirmation | 


# **get_installations_remove_confirmation**
> List[InstallationRemoveConfirmationResponse] get_installations_remove_confirmation(installations_ids=installations_ids)



Installation removal confirmation check

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.installation_remove_confirmation_response import InstallationRemoveConfirmationResponse
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
    api_instance = plesk_wp_toolkit_client.RemoverApi(api_client)
    installations_ids = [[1,3,5]] # List[int] | Array with installation IDs for filter (optional)

    try:
        api_response = api_instance.get_installations_remove_confirmation(installations_ids=installations_ids)
        print("The response of RemoverApi->get_installations_remove_confirmation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RemoverApi->get_installations_remove_confirmation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **installations_ids** | [**List[int]**](int.md)| Array with installation IDs for filter | [optional] 

### Return type

[**List[InstallationRemoveConfirmationResponse]**](InstallationRemoveConfirmationResponse.md)

### Authorization

[httpBasic](../README.md#httpBasic), [pleskApiToken](../README.md#pleskApiToken)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Installation removal confirmation |  -  |
**400** | Bad Request |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

