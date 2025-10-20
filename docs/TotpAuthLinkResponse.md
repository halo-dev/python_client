# TotpAuthLinkResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**auth_link** | **str** | QR Code with base64 encoded. | [optional] 
**raw_secret** | **str** |  | [optional] 

## Example

```python
from halo_client.models.totp_auth_link_response import TotpAuthLinkResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TotpAuthLinkResponse from a JSON string
totp_auth_link_response_instance = TotpAuthLinkResponse.from_json(json)
# print the JSON string representation of the object
print(TotpAuthLinkResponse.to_json())

# convert the object into a dict
totp_auth_link_response_dict = totp_auth_link_response_instance.to_dict()
# create an instance of TotpAuthLinkResponse from a dict
totp_auth_link_response_from_dict = TotpAuthLinkResponse.from_dict(totp_auth_link_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


