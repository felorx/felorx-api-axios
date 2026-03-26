# VerifyReceiptResult

校验结果

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [readonly] [default to undefined]
**creationTime** | **string** |  | [optional] [readonly] [default to undefined]
**creatorId** | **string** |  | [optional] [readonly] [default to undefined]
**lastModificationTime** | **string** |  | [optional] [default to undefined]
**lastModifierId** | **string** |  | [optional] [default to undefined]
**isDeleted** | **boolean** |  | [optional] [default to undefined]
**deleterId** | **string** |  | [optional] [default to undefined]
**deletionTime** | **string** |  | [optional] [default to undefined]
**deleter** | [**IdentityUser**](IdentityUser.md) |  | [optional] [default to undefined]
**creator** | [**IdentityUser**](IdentityUser.md) |  | [optional] [default to undefined]
**lastModifier** | [**IdentityUser**](IdentityUser.md) |  | [optional] [default to undefined]
**orderId** | **string** |  | [optional] [default to undefined]
**receiptData** | **string** |  | [optional] [default to undefined]
**platform** | [**AppPlatform**](AppPlatform.md) |  | [optional] [default to undefined]
**deviceToken** | **string** |  | [optional] [default to undefined]
**ok** | **boolean** |  | [optional] [default to undefined]
**statusCode** | **string** |  | [optional] [default to undefined]
**message** | **string** |  | [optional] [default to undefined]
**resultData** | **string** |  | [optional] [default to undefined]
**recordId** | **string** |  | [optional] [default to undefined]
**appleVerifyReceiptResult** | [**AppleVerifyReceiptResult**](AppleVerifyReceiptResult.md) |  | [optional] [default to undefined]

## Example

```typescript
import { VerifyReceiptResult } from 'puupee-api';

const instance: VerifyReceiptResult = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    deleter,
    creator,
    lastModifier,
    orderId,
    receiptData,
    platform,
    deviceToken,
    ok,
    statusCode,
    message,
    resultData,
    recordId,
    appleVerifyReceiptResult,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
