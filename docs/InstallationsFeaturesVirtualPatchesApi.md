# plesk_wp_toolkit_client.InstallationsFeaturesVirtualPatchesApi

All URIs are relative to *https://example.com/api/modules/wp-toolkit*

Method | HTTP request | Description
------------- | ------------- | -------------
[**update_virtual_patches_protection_status**](InstallationsFeaturesVirtualPatchesApi.md#update_virtual_patches_protection_status) | **POST** /v1/features/virtual-patches/protector | 


# **update_virtual_patches_protection_status**
> BackgroundTaskWithUrlResponse update_virtual_patches_protection_status(virtual_patches_protector_request, dry_run=dry_run)



Enable or disable vulnerability protection on WordPress installations

### Example

* Basic Authentication (httpBasic):
* Api Key Authentication (pleskApiToken):

```python
import plesk_wp_toolkit_client
from plesk_wp_toolkit_client.models.background_task_with_url_response import BackgroundTaskWithUrlResponse
from plesk_wp_toolkit_client.models.virtual_patches_protector_request import VirtualPatchesProtectorRequest
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
    api_instance = plesk_wp_toolkit_client.InstallationsFeaturesVirtualPatchesApi(api_client)
    virtual_patches_protector_request = plesk_wp_toolkit_client.VirtualPatchesProtectorRequest() # VirtualPatchesProtectorRequest | 
    dry_run = True # bool | Validate license limits, and service plan or package limits (optional)

    try:
        api_response = api_instance.update_virtual_patches_protection_status(virtual_patches_protector_request, dry_run=dry_run)
        print("The response of InstallationsFeaturesVirtualPatchesApi->update_virtual_patches_protection_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstallationsFeaturesVirtualPatchesApi->update_virtual_patches_protection_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **virtual_patches_protector_request** | [**VirtualPatchesProtectorRequest**](VirtualPatchesProtectorRequest.md)|  | 
 **dry_run** | **bool**| Validate license limits, and service plan or package limits | [optional] 

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
**204** | No Content |  -  |
**422** | Validation error |  -  |
**400** | Bad Request |  -  |
**401** | Unauthorized |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

