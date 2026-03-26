# AppPricingItemDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**creationTime** | **string** |  | [optional] [default to undefined]
**creatorId** | **string** |  | [optional] [default to undefined]
**lastModificationTime** | **string** |  | [optional] [default to undefined]
**lastModifierId** | **string** |  | [optional] [default to undefined]
**isDeleted** | **boolean** |  | [optional] [default to undefined]
**deleterId** | **string** |  | [optional] [default to undefined]
**deletionTime** | **string** |  | [optional] [default to undefined]
**key** | **string** | 键值, 例如: Seat, SingleFileMaxSize, UserStorageSize, MaxPuupeeCount, 见 AppPricingItemKeys.cs | [optional] [default to undefined]
**name** | **string** | 名称: 坐席 | [optional] [default to undefined]
**description** | **string** | 描述, 使用 Markdown 格式, 允许包含图片 | [optional] [default to undefined]
**linkUrl** | **string** | 链接地址 | [optional] [default to undefined]
**display** | **string** | 显示模板: 包括{0}个坐席 | [optional] [default to undefined]
**isAvailable** | **boolean** | 是否可用 | [optional] [default to undefined]
**sortIndex** | **number** | 排序 | [optional] [default to undefined]

## Example

```typescript
import { AppPricingItemDto } from 'puupee-api';

const instance: AppPricingItemDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    key,
    name,
    description,
    linkUrl,
    display,
    isAvailable,
    sortIndex,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
