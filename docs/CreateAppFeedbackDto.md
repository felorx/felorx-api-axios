# CreateAppFeedbackDto

创建应用反馈DTO

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appId** | **string** | 应用ID | [default to undefined]
**content** | **string** | 反馈内容 | [default to undefined]
**type** | [**AppFeedbackType**](AppFeedbackType.md) |  | [default to undefined]
**contact** | **string** | 联系方式（可选） | [optional] [default to undefined]
**deviceInfo** | **string** | 设备信息（可选） | [optional] [default to undefined]
**appVersion** | **string** | 应用版本（可选） | [optional] [default to undefined]

## Example

```typescript
import { CreateAppFeedbackDto } from 'puupee-api';

const instance: CreateAppFeedbackDto = {
    appId,
    content,
    type,
    contact,
    deviceInfo,
    appVersion,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
