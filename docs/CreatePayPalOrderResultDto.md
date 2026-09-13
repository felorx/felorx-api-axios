# CreatePayPalOrderResultDto

创建 PayPal 订单结果

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**orderId** | **string** | 本系统订单 ID | [optional] [default to undefined]
**payPalOrderId** | **string** | PayPal 订单 ID（供前端按钮使用） | [optional] [default to undefined]
**payPalSubscriptionId** | **string** | PayPal 订阅 ID（自动续费场景） | [optional] [default to undefined]
**approvalUrl** | **string** | PayPal approve 链接，可用于不使用 JS SDK 的桌面端跳转。 | [optional] [default to undefined]
**checkoutKind** | **string** | order&#x3D;一次性订单，subscription&#x3D;自动续费订阅。 | [optional] [default to undefined]

## Example

```typescript
import { CreatePayPalOrderResultDto } from 'felorx-api';

const instance: CreatePayPalOrderResultDto = {
    orderId,
    payPalOrderId,
    payPalSubscriptionId,
    approvalUrl,
    checkoutKind,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
