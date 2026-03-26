# AppleVerifyReceiptResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**environment** | **string** |  | [optional] [default to undefined]
**is_retryable** | **boolean** |  | [optional] [default to undefined]
**status** | **number** | 订阅订单状态 | [optional] [default to undefined]
**latest_receipt_info** | [**Array&lt;LatestReceiptInfo&gt;**](LatestReceiptInfo.md) |  | [optional] [default to undefined]
**latest_receipt** | **string** |  | [optional] [default to undefined]
**pending_renewal_info** | [**Array&lt;PendingRenewalInfo&gt;**](PendingRenewalInfo.md) |  | [optional] [default to undefined]
**receipt** | [**Receipt**](Receipt.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AppleVerifyReceiptResult } from 'puupee-api';

const instance: AppleVerifyReceiptResult = {
    environment,
    is_retryable,
    status,
    latest_receipt_info,
    latest_receipt,
    pending_renewal_info,
    receipt,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
