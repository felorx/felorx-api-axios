# AppPlanPriceDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**creationTime** | **string** |  | [optional] [default to undefined]
**creatorId** | **string** |  | [optional] [default to undefined]
**lastModificationTime** | **string** |  | [optional] [default to undefined]
**lastModifierId** | **string** |  | [optional] [default to undefined]
**isDeleted** | **boolean** |  | [optional] [default to undefined]
**deleterId** | **string** |  | [optional] [default to undefined]
**deletionTime** | **string** |  | [optional] [default to undefined]
**appId** | **string** |  | [optional] [default to undefined]
**pricingId** | **string** |  | [optional] [default to undefined]
**period** | [**SubBillingPeriod**](SubBillingPeriod.md) |  | [optional] [default to undefined]
**mode** | [**BillingMode**](BillingMode.md) |  | [optional] [default to undefined]
**market** | [**BillingMarket**](BillingMarket.md) |  | [optional] [default to undefined]
**currency** | **string** |  | [optional] [default to undefined]
**amount** | **number** |  | [optional] [default to undefined]
**discountAmount** | **number** |  | [optional] [default to undefined]
**effectiveAmount** | **number** |  | [optional] [default to undefined]
**durationDays** | **number** |  | [optional] [default to undefined]
**isEnabled** | **boolean** |  | [optional] [default to undefined]
**sortIndex** | **number** |  | [optional] [default to undefined]
**displayName** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { AppPlanPriceDto } from 'felorx-api';

const instance: AppPlanPriceDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    appId,
    pricingId,
    period,
    mode,
    market,
    currency,
    amount,
    discountAmount,
    effectiveAmount,
    durationDays,
    isEnabled,
    sortIndex,
    displayName,
    description,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
