# CapturePayPalOrderDto

捕获 PayPal 订单请求

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**payPalOrderId** | **string** | PayPal 订单 ID | [optional] [default to undefined]
**payPalSubscriptionId** | **string** | PayPal 订阅 ID。自动续费场景使用该字段。 | [optional] [default to undefined]

## Example

```typescript
import { CapturePayPalOrderDto } from 'felorx-api';

const instance: CapturePayPalOrderDto = {
    payPalOrderId,
    payPalSubscriptionId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
