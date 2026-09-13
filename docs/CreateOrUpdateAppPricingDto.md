# CreateOrUpdateAppPricingDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**naming** | [**AppPriceNaming**](AppPriceNaming.md) |  | [optional] [default to undefined]
**description** | **string** | 简单描述  适用于个人网站和任何想用基本的聊天方式与游客交流的人。  适用于希望改善客户关系的早期创业公司。  为需要全功能解决方案与客户沟通的公司而设。 | [optional] [default to undefined]
**appId** | **string** | APPID | [optional] [default to undefined]
**sortIndex** | **number** | 排序 | [optional] [default to undefined]
**items** | [**Array&lt;AppPricingItemValueDto&gt;**](AppPricingItemValueDto.md) | 收费点 | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateAppPricingDto } from 'felorx-api';

const instance: CreateOrUpdateAppPricingDto = {
    naming,
    description,
    appId,
    sortIndex,
    items,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
