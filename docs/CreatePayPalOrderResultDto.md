# CreatePayPalOrderResultDto

创建 PayPal 订单结果

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**orderId** | **string** | 本系统订单 ID | [optional] [default to undefined]
**payPalOrderId** | **string** | PayPal 订单 ID（供前端按钮使用） | [optional] [default to undefined]

## Example

```typescript
import { CreatePayPalOrderResultDto } from 'puupee-api';

const instance: CreatePayPalOrderResultDto = {
    orderId,
    payPalOrderId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
