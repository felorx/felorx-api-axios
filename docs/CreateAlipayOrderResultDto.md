# CreateAlipayOrderResultDto

创建支付宝一次性支付订单结果。

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**orderId** | **string** | 本系统订单 ID。 | [optional] [default to undefined]
**outTradeNo** | **string** | 支付宝商户订单号 out_trade_no。 | [optional] [default to undefined]
**checkoutMode** | **string** | 支付入口：page、wap 或 app。 | [optional] [default to undefined]
**paymentForm** | **string** | 电脑/手机网站支付的 HTML 表单，可由 Web 前端写入页面并提交。 | [optional] [default to undefined]
**paymentUrl** | **string** | 从支付表单中提取出的跳转地址。桌面和 Android 可用外部浏览器打开。 | [optional] [default to undefined]
**orderString** | **string** | App 支付订单串，原生客户端接支付宝 App SDK 时使用。 | [optional] [default to undefined]

## Example

```typescript
import { CreateAlipayOrderResultDto } from 'felorx-api';

const instance: CreateAlipayOrderResultDto = {
    orderId,
    outTradeNo,
    checkoutMode,
    paymentForm,
    paymentUrl,
    orderString,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
