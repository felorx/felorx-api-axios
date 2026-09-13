# CreateOrUpdateAppPlanPriceDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appId** | **string** |  | [optional] [default to undefined]
**pricingId** | **string** |  | [optional] [default to undefined]
**period** | [**SubBillingPeriod**](SubBillingPeriod.md) |  | [optional] [default to undefined]
**mode** | [**BillingMode**](BillingMode.md) |  | [optional] [default to undefined]
**market** | [**BillingMarket**](BillingMarket.md) |  | [optional] [default to undefined]
**currency** | **string** |  | [optional] [default to undefined]
**amount** | **number** |  | [optional] [default to undefined]
**discountAmount** | **number** |  | [optional] [default to undefined]
**durationDays** | **number** |  | [optional] [default to undefined]
**isEnabled** | **boolean** |  | [optional] [default to undefined]
**sortIndex** | **number** |  | [optional] [default to undefined]
**displayName** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateAppPlanPriceDto } from 'felorx-api';

const instance: CreateOrUpdateAppPlanPriceDto = {
    appId,
    pricingId,
    period,
    mode,
    market,
    currency,
    amount,
    discountAmount,
    durationDays,
    isEnabled,
    sortIndex,
    displayName,
    description,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
