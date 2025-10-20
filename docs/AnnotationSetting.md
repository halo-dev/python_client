# AnnotationSetting


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**spec** | [**AnnotationSettingSpec**](AnnotationSettingSpec.md) |  | 

## Example

```python
from halo_client.models.annotation_setting import AnnotationSetting

# TODO update the JSON string below
json = "{}"
# create an instance of AnnotationSetting from a JSON string
annotation_setting_instance = AnnotationSetting.from_json(json)
# print the JSON string representation of the object
print(AnnotationSetting.to_json())

# convert the object into a dict
annotation_setting_dict = annotation_setting_instance.to_dict()
# create an instance of AnnotationSetting from a dict
annotation_setting_from_dict = AnnotationSetting.from_dict(annotation_setting_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


