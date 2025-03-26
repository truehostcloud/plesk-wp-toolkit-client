# InstallationStubResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**admin** | [**AdminSettings**](AdminSettings.md) |  | 
**database** | [**DatabaseSettings**](DatabaseSettings.md) |  | 
**protocol** | [**ParameterWithChoices**](ParameterWithChoices.md) |  | 
**title** | [**InstallationStubResponseTitle**](InstallationStubResponseTitle.md) |  | 
**installation_path** | [**InstallationStubResponseInstallationPath**](InstallationStubResponseInstallationPath.md) |  | 
**auto_update** | [**AutoUpdateSettings**](AutoUpdateSettings.md) |  | 
**language** | [**ParameterWithChoices**](ParameterWithChoices.md) |  | 
**domain** | [**ParameterWithChoices**](ParameterWithChoices.md) |  | 
**version** | [**ParameterWithChoices**](ParameterWithChoices.md) |  | 
**set** | [**ParameterWithChoices**](ParameterWithChoices.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_stub_response import InstallationStubResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationStubResponse from a JSON string
installation_stub_response_instance = InstallationStubResponse.from_json(json)
# print the JSON string representation of the object
print(InstallationStubResponse.to_json())

# convert the object into a dict
installation_stub_response_dict = installation_stub_response_instance.to_dict()
# create an instance of InstallationStubResponse from a dict
installation_stub_response_from_dict = InstallationStubResponse.from_dict(installation_stub_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


