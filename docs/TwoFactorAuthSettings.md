# TwoFactorAuthSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Check if 2FA is available. | [optional] 
**email_verified** | **bool** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**totp_configured** | **bool** |  | [optional] 

## Example

```python
from halo_client.models.two_factor_auth_settings import TwoFactorAuthSettings

# TODO update the JSON string below
json = "{}"
# create an instance of TwoFactorAuthSettings from a JSON string
two_factor_auth_settings_instance = TwoFactorAuthSettings.from_json(json)
# print the JSON string representation of the object
print(TwoFactorAuthSettings.to_json())

# convert the object into a dict
two_factor_auth_settings_dict = two_factor_auth_settings_instance.to_dict()
# create an instance of TwoFactorAuthSettings from a dict
two_factor_auth_settings_from_dict = TwoFactorAuthSettings.from_dict(two_factor_auth_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


