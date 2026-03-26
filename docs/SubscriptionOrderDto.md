# SubscriptionOrderDto


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
**type** | [**SubscriptionOrderType**](SubscriptionOrderType.md) |  | [optional] [default to undefined]
**status** | [**SubscriptionOrderStatus**](SubscriptionOrderStatus.md) |  | [optional] [default to undefined]
**appId** | **string** |  | [optional] [default to undefined]
**pricingId** | **string** |  | [optional] [default to undefined]
**productId** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { SubscriptionOrderDto } from 'puupee-api';

const instance: SubscriptionOrderDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    type,
    status,
    appId,
    pricingId,
    productId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
