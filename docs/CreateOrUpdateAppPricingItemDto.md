# CreateOrUpdateAppPricingItemDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | 名称: 坐席 | [optional] [default to undefined]
**description** | **string** | 描述, 使用 Markdown 格式, 允许包含图片 | [optional] [default to undefined]
**linkUrl** | **string** | 链接地址 | [optional] [default to undefined]
**display** | **string** | 显示模板: 包括{0}个坐席 | [optional] [default to undefined]
**sortIndex** | **number** | 排序 | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateAppPricingItemDto } from 'puupee-api';

const instance: CreateOrUpdateAppPricingItemDto = {
    name,
    description,
    linkUrl,
    display,
    sortIndex,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
