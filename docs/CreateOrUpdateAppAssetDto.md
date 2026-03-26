# CreateOrUpdateAppAssetDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appId** | **string** |  | [optional] [default to undefined]
**appLocaleId** | **string** |  | [optional] [default to undefined]
**appFeatureId** | **string** |  | [optional] [default to undefined]
**assetType** | [**AppAssetType**](AppAssetType.md) |  | [optional] [default to undefined]
**deviceType** | [**AppAssetDeviceType**](AppAssetDeviceType.md) |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**sort** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateAppAssetDto } from 'puupee-api';

const instance: CreateOrUpdateAppAssetDto = {
    appId,
    appLocaleId,
    appFeatureId,
    assetType,
    deviceType,
    url,
    sort,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
