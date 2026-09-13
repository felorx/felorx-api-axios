# CreateOrUpdateAppPricingItemDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key** | **string** | 键值, 例如: Seat, MaxListCount（见 AppPricingItemKeys） | [optional] [default to undefined]
**appId** | **string** | 所属应用 | [optional] [default to undefined]
**name** | **string** | 名称: 坐席 | [optional] [default to undefined]
**description** | **string** | 描述, 使用 Markdown 格式, 允许包含图片 | [optional] [default to undefined]
**linkUrl** | **string** | 链接地址 | [optional] [default to undefined]
**display** | **string** | 显示模板: 包括{0}个坐席 | [optional] [default to undefined]
**sortIndex** | **number** | 排序 | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateAppPricingItemDto } from 'felorx-api';

const instance: CreateOrUpdateAppPricingItemDto = {
    key,
    appId,
    name,
    description,
    linkUrl,
    display,
    sortIndex,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
