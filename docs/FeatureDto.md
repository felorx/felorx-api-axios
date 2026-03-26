# FeatureDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**displayName** | **string** |  | [optional] [default to undefined]
**value** | **string** |  | [optional] [default to undefined]
**provider** | [**FeatureProviderDto**](FeatureProviderDto.md) |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**valueType** | [**IStringValueType**](IStringValueType.md) |  | [optional] [default to undefined]
**depth** | **number** |  | [optional] [default to undefined]
**parentName** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FeatureDto } from 'puupee-api';

const instance: FeatureDto = {
    name,
    displayName,
    value,
    provider,
    description,
    valueType,
    depth,
    parentName,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
