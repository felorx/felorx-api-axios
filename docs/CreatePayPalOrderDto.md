# CreatePayPalOrderDto

创建 PayPal 订单请求

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appId** | **string** | 应用 ID | [optional] [default to undefined]
**pricingId** | **string** | 定价方案 ID | [optional] [default to undefined]
**planType** | **string** | 计划类型：month&#x3D;月度, year&#x3D;年度 | [optional] [default to undefined]

## Example

```typescript
import { CreatePayPalOrderDto } from 'puupee-api';

const instance: CreatePayPalOrderDto = {
    appId,
    pricingId,
    planType,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
