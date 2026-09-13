# CreateAlipayOrderDto

创建支付宝一次性支付订单请求。

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appId** | **string** | 应用 ID。 | [optional] [default to undefined]
**pricingId** | **string** | 定价方案 ID。 | [optional] [default to undefined]
**planType** | **string** | 计划类型：month&#x3D;月度, year&#x3D;年度, three_year&#x3D;三年, lifetime&#x3D;终身。 | [optional] [default to undefined]
**checkoutMode** | **string** | 支付入口：page&#x3D;电脑网站支付, wap&#x3D;手机网站支付, app&#x3D;App 支付订单串。 | [optional] [default to undefined]
**returnUrl** | **string** | 支付完成后的同步跳转地址。 | [optional] [default to undefined]
**quitUrl** | **string** | 手机网站支付中用户取消后的返回地址。 | [optional] [default to undefined]

## Example

```typescript
import { CreateAlipayOrderDto } from 'felorx-api';

const instance: CreateAlipayOrderDto = {
    appId,
    pricingId,
    planType,
    checkoutMode,
    returnUrl,
    quitUrl,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
