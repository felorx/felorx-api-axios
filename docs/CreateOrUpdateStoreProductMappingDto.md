# CreateOrUpdateStoreProductMappingDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**appId** | **string** |  | [optional] [default to undefined]
**pricingId** | **string** |  | [optional] [default to undefined]
**planPriceId** | **string** |  | [optional] [default to undefined]
**provider** | [**BillingProvider**](BillingProvider.md) |  | [optional] [default to undefined]
**platform** | [**AppPlatform**](AppPlatform.md) |  | [optional] [default to undefined]
**period** | [**SubBillingPeriod**](SubBillingPeriod.md) |  | [optional] [default to undefined]
**storeProductId** | **string** |  | [optional] [default to undefined]
**externalProductId** | **string** |  | [optional] [default to undefined]
**environment** | **string** |  | [optional] [default to undefined]
**isEnabled** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateStoreProductMappingDto } from 'felorx-api';

const instance: CreateOrUpdateStoreProductMappingDto = {
    id,
    appId,
    pricingId,
    planPriceId,
    provider,
    platform,
    period,
    storeProductId,
    externalProductId,
    environment,
    isEnabled,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
