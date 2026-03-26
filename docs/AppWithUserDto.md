# AppWithUserDto


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
**name** | **string** |  | [optional] [default to undefined]
**displayName** | **string** | 根据 Accept-Language 解析的展示标题（非持久化字段，来自语言包）。 | [optional] [default to undefined]
**framework** | [**AppFramework**](AppFramework.md) |  | [optional] [default to undefined]
**appType** | [**AppType**](AppType.md) |  | [optional] [default to undefined]
**description** | **string** | 根据 Accept-Language 解析的短描述（非持久化字段）。 | [optional] [default to undefined]
**icon** | **string** | 根据 Accept-Language 解析的图标存储键或 URL（非持久化字段）。 | [optional] [default to undefined]
**homePage** | **string** | 产品首页 | [optional] [default to undefined]
**sortIndex** | **number** | 显示排序 | [optional] [default to undefined]
**gitRepository** | **string** |  | [optional] [default to undefined]
**gitRepositoryType** | [**GitRepositoryType**](GitRepositoryType.md) |  | [optional] [default to undefined]
**isEnabled** | **boolean** |  | [optional] [default to undefined]
**isPublished** | **boolean** | 是否已经发布, 决定了是否给终端用户看见, 主要有一些 APP 自己使用 | [optional] [default to undefined]
**webhookUrl** | **string** | Webhook Url 各种事件回调地址 | [optional] [default to undefined]
**businessDomain** | **string** | 业务域名 | [optional] [default to undefined]
**businessUrl** | **string** | 业务地址 | [optional] [default to undefined]
**subscriptionPlatforms** | **string** | 可以订阅的平台 Platform 枚举, 并用\&quot;,\&quot;分割 | [optional] [default to undefined]
**freePlatforms** | **string** | 暂时免费的平台, 付费功能免费用的平台, 用\&quot;,\&quot;分割 | [optional] [default to undefined]
**specJsonSchema** | **string** | 声明格式 | [optional] [default to undefined]
**defaultStorageSize** | **number** | 默认存储空间大小 | [optional] [default to undefined]
**defaultSingleFileMaxSize** | **number** | 默认单文件最大大小 | [optional] [default to undefined]
**latestReleases** | [**Array&lt;AppReleaseDto&gt;**](AppReleaseDto.md) |  | [optional] [default to undefined]
**creator** | [**IdentityUserDto**](IdentityUserDto.md) |  | [optional] [default to undefined]
**subscribed** | **boolean** | 是否已经订阅 | [optional] [default to undefined]

## Example

```typescript
import { AppWithUserDto } from 'puupee-api';

const instance: AppWithUserDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    name,
    displayName,
    framework,
    appType,
    description,
    icon,
    homePage,
    sortIndex,
    gitRepository,
    gitRepositoryType,
    isEnabled,
    isPublished,
    webhookUrl,
    businessDomain,
    businessUrl,
    subscriptionPlatforms,
    freePlatforms,
    specJsonSchema,
    defaultStorageSize,
    defaultSingleFileMaxSize,
    latestReleases,
    creator,
    subscribed,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
