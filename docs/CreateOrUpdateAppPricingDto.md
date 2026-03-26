# CreateOrUpdateAppPricingDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**naming** | [**AppPriceNaming**](AppPriceNaming.md) |  | [optional] [default to undefined]
**monthProductId** | **string** | 商店订阅产品 ID | [optional] [default to undefined]
**yearProductId** | **string** | 商店订阅产品 ID | [optional] [default to undefined]
**description** | **string** | 简单描述  适用于个人网站和任何想用基本的聊天方式与游客交流的人。  适用于希望改善客户关系的早期创业公司。  为需要全功能解决方案与客户沟通的公司而设。 | [optional] [default to undefined]
**appId** | **string** | APPID | [optional] [default to undefined]
**monthPrice** | **number** | 价格 | [optional] [default to undefined]
**monthDiscount** | **number** | 折扣 | [optional] [default to undefined]
**monthDiscountPrice** | **number** | 折扣后价格 DiscountPrice &#x3D; Price * Discount | [optional] [default to undefined]
**monthDiscountStartAt** | **string** | 折扣开始时间 | [optional] [default to undefined]
**monthDiscountEndAt** | **string** | 折扣结束时间 | [optional] [default to undefined]
**yearPrice** | **number** | 价格 | [optional] [default to undefined]
**yearDiscount** | **number** | 折扣 | [optional] [default to undefined]
**yearDiscountPrice** | **number** | 折扣后价格 DiscountPrice &#x3D; Price * Discount | [optional] [default to undefined]
**yearDiscountStartAt** | **string** | 折扣开始时间 | [optional] [default to undefined]
**yearDiscountEndAt** | **string** | 折扣结束时间 | [optional] [default to undefined]
**sortIndex** | **number** | 排序 | [optional] [default to undefined]
**items** | [**Array&lt;AppPricingItemValueDto&gt;**](AppPricingItemValueDto.md) | 收费点 | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateAppPricingDto } from 'puupee-api';

const instance: CreateOrUpdateAppPricingDto = {
    naming,
    monthProductId,
    yearProductId,
    description,
    appId,
    monthPrice,
    monthDiscount,
    monthDiscountPrice,
    monthDiscountStartAt,
    monthDiscountEndAt,
    yearPrice,
    yearDiscount,
    yearDiscountPrice,
    yearDiscountStartAt,
    yearDiscountEndAt,
    sortIndex,
    items,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
