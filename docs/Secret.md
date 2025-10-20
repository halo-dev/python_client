# Secret

Secret is a small piece of sensitive data which should be kept secret, such as a password,  a token, or a key.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** |  | 
**data** | **Dict[str, bytearray]** | &lt;p&gt;The total bytes of the values in  the Data field must be less than {@link run.halo.app.extension.Secret#MAX_SECRET_SIZE #MAX_SECRET_SIZE} bytes.&lt;/p&gt;  &lt;p&gt;&lt;code&gt;data&lt;/code&gt; contains the secret data. Each key must consist of alphanumeric  characters, &#39;-&#39;, &#39;_&#39; or &#39;.&#39;. The serialized form of the secret data is a  base64 encoded string, representing the arbitrary (possibly non-string)  data value here. Described in  &lt;a href&#x3D;\&quot;https://tools.ietf.org/html/rfc4648#section-4\&quot;&gt;rfc4648#section-4&lt;/a&gt;  &lt;/p&gt; | [optional] 
**kind** | **str** |  | 
**metadata** | [**Metadata**](Metadata.md) |  | 
**string_data** | **Dict[str, str]** | &lt;code&gt;stringData&lt;/code&gt; allows specifying non-binary secret data in string form.  It is provided as a write-only input field for convenience.  All keys and values are merged into the data field on write, overwriting any existing  values.  The stringData field is never output when reading from the API. | [optional] 
**type** | **str** | Used to facilitate programmatic handling of secret data.  More info:  &lt;a href&#x3D;\&quot;https://kubernetes.io/docs/concepts/configuration/secret/#secret-types\&quot;&gt;secret-types&lt;/a&gt; | [optional] 

## Example

```python
from halo_client.models.secret import Secret

# TODO update the JSON string below
json = "{}"
# create an instance of Secret from a JSON string
secret_instance = Secret.from_json(json)
# print the JSON string representation of the object
print(Secret.to_json())

# convert the object into a dict
secret_dict = secret_instance.to_dict()
# create an instance of Secret from a dict
secret_from_dict = Secret.from_dict(secret_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


