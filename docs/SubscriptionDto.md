# SubscriptionDto


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
**expireAt** | **string** | 会员过期时间 | [optional] [default to undefined]
**appId** | **string** | 应用 ID | [optional] [default to undefined]
**priceNaming** | [**AppPriceNaming**](AppPriceNaming.md) |  | [optional] [default to undefined]
**pricingId** | **string** |  | [optional] [default to undefined]
**planPriceId** | **string** |  | [optional] [default to undefined]
**provider** | [**BillingProvider**](BillingProvider.md) |  | [optional] [default to undefined]
**billingPeriod** | [**SubBillingPeriod**](SubBillingPeriod.md) |  | [optional] [default to undefined]
**billingMode** | [**BillingMode**](BillingMode.md) |  | [optional] [default to undefined]
**status** | [**SubscriptionEntitlementStatus**](SubscriptionEntitlementStatus.md) |  | [optional] [default to undefined]
**isLifetime** | **boolean** |  | [optional] [default to undefined]
**externalSubscriptionId** | **string** |  | [optional] [default to undefined]
**lastVerifiedAt** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { SubscriptionDto } from 'felorx-api';

const instance: SubscriptionDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    expireAt,
    appId,
    priceNaming,
    pricingId,
    planPriceId,
    provider,
    billingPeriod,
    billingMode,
    status,
    isLifetime,
    externalSubscriptionId,
    lastVerifiedAt,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
