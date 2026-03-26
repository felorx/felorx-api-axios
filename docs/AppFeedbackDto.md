# AppFeedbackDto

应用反馈DTO

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
**appId** | **string** | 应用ID | [optional] [default to undefined]
**appName** | **string** | 应用名称 | [optional] [default to undefined]
**content** | **string** | 反馈内容 | [optional] [default to undefined]
**type** | [**AppFeedbackType**](AppFeedbackType.md) |  | [optional] [default to undefined]
**status** | [**AppFeedbackStatus**](AppFeedbackStatus.md) |  | [optional] [default to undefined]
**contact** | **string** | 联系方式 | [optional] [default to undefined]
**deviceInfo** | **string** | 设备信息 | [optional] [default to undefined]
**appVersion** | **string** | 应用版本 | [optional] [default to undefined]
**reply** | **string** | 回复内容 | [optional] [default to undefined]
**repliedAt** | **string** | 回复时间 | [optional] [default to undefined]

## Example

```typescript
import { AppFeedbackDto } from 'puupee-api';

const instance: AppFeedbackDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    appId,
    appName,
    content,
    type,
    status,
    contact,
    deviceInfo,
    appVersion,
    reply,
    repliedAt,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
