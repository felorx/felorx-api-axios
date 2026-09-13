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
**attachmentKeys** | **Array&lt;string&gt;** | 截图/图片附件（对象存储 key，最多 5 个） | [optional] [default to undefined]

## Example

```typescript
import { CreateAppFeedbackDto } from 'felorx-api';

const instance: CreateAppFeedbackDto = {
    appId,
    content,
    type,
    contact,
    deviceInfo,
    appVersion,
    attachmentKeys,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
