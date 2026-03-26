# UserStorageDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appId** | **string** | 所属应用 | [optional] [default to undefined]
**appName** | **string** | 应用名称 | [optional] [default to undefined]
**priceNaming** | [**AppPriceNaming**](AppPriceNaming.md) |  | [optional] [default to undefined]
**size** | **number** | 用户存储容量 | [optional] [default to undefined]
**currentSize** | **number** | 当前使用大小 | [optional] [default to undefined]
**totalCount** | **number** |  | [optional] [default to undefined]
**singleFileMaxSize** | **number** | 单文件最大大小 | [optional] [default to undefined]
**expireAt** | **string** | 过期时间, 为空表示永久有效, 一般是订阅产品的过期时间 | [optional] [default to undefined]
**items** | [**Array&lt;UserStorageItemDto&gt;**](UserStorageItemDto.md) |  | [optional] [default to undefined]

## Example

```typescript
import { UserStorageDto } from 'puupee-api';

const instance: UserStorageDto = {
    appId,
    appName,
    priceNaming,
    size,
    currentSize,
    totalCount,
    singleFileMaxSize,
    expireAt,
    items,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
