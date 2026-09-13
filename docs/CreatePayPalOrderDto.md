# CreatePayPalOrderDto

创建 PayPal 订单请求

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appId** | **string** | 应用 ID | [optional] [default to undefined]
**pricingId** | **string** | 定价方案 ID | [optional] [default to undefined]
**planType** | **string** | 计划类型：month&#x3D;月度, year&#x3D;年度, three_year&#x3D;三年, lifetime&#x3D;终身 | [optional] [default to undefined]
**returnUrl** | **string** | 支付完成后返回地址，桌面端可传深链。 | [optional] [default to undefined]
**cancelUrl** | **string** | 支付取消后返回地址，桌面端可传深链。 | [optional] [default to undefined]

## Example

```typescript
import { CreatePayPalOrderDto } from 'felorx-api';

const instance: CreatePayPalOrderDto = {
    appId,
    pricingId,
    planType,
    returnUrl,
    cancelUrl,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
