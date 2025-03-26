# InstallationFeatures


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**wp_cron_takeover** | [**InstallationWpCron**](InstallationWpCron.md) |  | 
**updates** | [**InstallationUpdates**](InstallationUpdates.md) |  | 
**restore_point** | [**InstallationRestorePoint**](InstallationRestorePoint.md) |  | 
**maintenance** | [**InstallationMaintenance**](InstallationMaintenance.md) |  | 
**hotlink_protection** | [**InstallationHotlinkProtection**](InstallationHotlinkProtection.md) |  | 
**security** | [**InstallationSecurity**](InstallationSecurity.md) |  | 
**nginx_caching** | [**InstallationNginxCaching**](InstallationNginxCaching.md) |  | 
**indexing** | [**InstallationIndexing**](InstallationIndexing.md) |  | 
**debug** | [**InstallationDebug**](InstallationDebug.md) |  | 
**password_protection** | [**InstallationPasswordProtection**](InstallationPasswordProtection.md) |  | 
**vulnerability** | [**InstallationVulnerability**](InstallationVulnerability.md) |  | 
**multiple_sites_management** | [**InstallationMultipleSitesManagement**](InstallationMultipleSitesManagement.md) |  | 
**clone** | [**InstallationClone**](InstallationClone.md) |  | 
**copy_data** | [**InstallationCopyData**](InstallationCopyData.md) |  | 
**credentials** | [**InstallationCredentials**](InstallationCredentials.md) |  | 
**backups** | [**InstallationBackups**](InstallationBackups.md) |  | 
**file_manager** | [**InstallationFileManager**](InstallationFileManager.md) |  | 
**action_log** | [**InstallationActionLog**](InstallationActionLog.md) |  | 
**remote_management** | [**InstallationRemoteManagement**](InstallationRemoteManagement.md) |  | 
**synchronize_site_url** | [**InstallationSynchronizeSiteUrl**](InstallationSynchronizeSiteUrl.md) |  | 
**malware_scan** | [**InstallationMalwareScan**](InstallationMalwareScan.md) |  | 
**php** | [**InstallationPhp**](InstallationPhp.md) |  | 
**integrity** | [**InstallationIntegrityFeature**](InstallationIntegrityFeature.md) |  | 
**plugins_block_list** | [**InstallationPluginsBlockList**](InstallationPluginsBlockList.md) |  | 
**virtual_patches** | [**InstallationVirtualPatches**](InstallationVirtualPatches.md) |  | 
**vulnerability_filtering** | [**InstallationVulnerabilityFiltering**](InstallationVulnerabilityFiltering.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_features import InstallationFeatures

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationFeatures from a JSON string
installation_features_instance = InstallationFeatures.from_json(json)
# print the JSON string representation of the object
print(InstallationFeatures.to_json())

# convert the object into a dict
installation_features_dict = installation_features_instance.to_dict()
# create an instance of InstallationFeatures from a dict
installation_features_from_dict = InstallationFeatures.from_dict(installation_features_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


