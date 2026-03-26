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

## Example

```typescript
import { SubscriptionDto } from 'puupee-api';

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
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
