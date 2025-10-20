# SettingSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**forms** | [**List[SettingForm]**](SettingForm.md) |  | 

## Example

```python
from halo_client.models.setting_spec import SettingSpec

# TODO update the JSON string below
json = "{}"
# create an instance of SettingSpec from a JSON string
setting_spec_instance = SettingSpec.from_json(json)
# print the JSON string representation of the object
print(SettingSpec.to_json())

# convert the object into a dict
setting_spec_dict = setting_spec_instance.to_dict()
# create an instance of SettingSpec from a dict
setting_spec_from_dict = SettingSpec.from_dict(setting_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


