# CreateOrUpdateAppDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**framework** | [**AppFramework**](AppFramework.md) |  | [optional] [default to undefined]
**appType** | [**AppType**](AppType.md) |  | [optional] [default to undefined]
**homePage** | **string** | 产品首页 | [optional] [default to undefined]
**sortIndex** | **number** | 显示排序 | [optional] [default to undefined]
**gitRepository** | **string** |  | [optional] [default to undefined]
**gitRepositoryType** | [**GitRepositoryType**](GitRepositoryType.md) |  | [optional] [default to undefined]
**isEnabled** | **boolean** |  | [optional] [default to undefined]
**webhookUrl** | **string** | Webhook Url 各种事件回调地址 | [optional] [default to undefined]
**businessDomain** | **string** | 业务域名 | [optional] [default to undefined]
**businessUrl** | **string** | 业务地址 | [optional] [default to undefined]
**subscriptionPlatforms** | **string** | 可以订阅的平台 Platform 枚举, 并用\&quot;,\&quot;分割 | [optional] [default to undefined]
**freePlatforms** | **string** | 暂时免费的平台, 付费功能免费用的平台, 用\&quot;,\&quot;分割 | [optional] [default to undefined]
**specJsonSchema** | **string** | 声明格式 | [optional] [default to undefined]
**defaultStorageSize** | **number** | 默认存储空间大小 | [optional] [default to undefined]
**defaultSingleFileMaxSize** | **number** | 默认单文件最大大小 | [optional] [default to undefined]
**isPublished** | **boolean** | 是否已经发布, 决定了是否给终端用户看见, 主要有一些 APP 自己使用 | [optional] [default to undefined]
**openClient** | [**CreateOpenIddictApplicationDto**](CreateOpenIddictApplicationDto.md) |  | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateAppDto } from 'puupee-api';

const instance: CreateOrUpdateAppDto = {
    name,
    framework,
    appType,
    homePage,
    sortIndex,
    gitRepository,
    gitRepositoryType,
    isEnabled,
    webhookUrl,
    businessDomain,
    businessUrl,
    subscriptionPlatforms,
    freePlatforms,
    specJsonSchema,
    defaultStorageSize,
    defaultSingleFileMaxSize,
    isPublished,
    openClient,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
