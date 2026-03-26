# VerifyReceiptDto


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
**orderId** | **string** |  | [default to undefined]
**receiptData** | **string** |  | [default to undefined]
**platform** | [**AppPlatform**](AppPlatform.md) |  | [default to undefined]
**deviceToken** | **string** |  | [default to undefined]

## Example

```typescript
import { VerifyReceiptDto } from 'puupee-api';

const instance: VerifyReceiptDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    orderId,
    receiptData,
    platform,
    deviceToken,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
