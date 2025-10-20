# SettingForm


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**form_schema** | **List[object]** |  | 
**group** | **str** |  | 
**label** | **str** |  | [optional] 

## Example

```python
from halo_client.models.setting_form import SettingForm

# TODO update the JSON string below
json = "{}"
# create an instance of SettingForm from a JSON string
setting_form_instance = SettingForm.from_json(json)
# print the JSON string representation of the object
print(SettingForm.to_json())

# convert the object into a dict
setting_form_dict = setting_form_instance.to_dict()
# create an instance of SettingForm from a dict
setting_form_from_dict = SettingForm.from_dict(setting_form_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


