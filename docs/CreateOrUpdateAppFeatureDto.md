# CreateOrUpdateAppFeatureDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appId** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**sort** | **number** |  | [optional] [default to undefined]
**featureLocales** | [**Array&lt;CreateOrUpdateAppFeatureLocaleDto&gt;**](CreateOrUpdateAppFeatureLocaleDto.md) |  | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateAppFeatureDto } from 'puupee-api';

const instance: CreateOrUpdateAppFeatureDto = {
    appId,
    name,
    sort,
    featureLocales,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
