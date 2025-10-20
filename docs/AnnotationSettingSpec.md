# AnnotationSettingSpec


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**form_schema** | **List[object]** |  | 
**target_ref** | [**GroupKind**](GroupKind.md) |  | 

## Example

```python
from halo_client.models.annotation_setting_spec import AnnotationSettingSpec

# TODO update the JSON string below
json = "{}"
# create an instance of AnnotationSettingSpec from a JSON string
annotation_setting_spec_instance = AnnotationSettingSpec.from_json(json)
# print the JSON string representation of the object
print(AnnotationSettingSpec.to_json())

# convert the object into a dict
annotation_setting_spec_dict = annotation_setting_spec_instance.to_dict()
# create an instance of AnnotationSettingSpec from a dict
annotation_setting_spec_from_dict = AnnotationSettingSpec.from_dict(annotation_setting_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


