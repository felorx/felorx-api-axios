# UpdateBuildRecordDto

更新构建记录DTO

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | [**BuildStatus**](BuildStatus.md) |  | [default to undefined]
**logs** | **string** | 构建日志 | [optional] [default to undefined]
**errorMessage** | **string** | 错误信息 | [optional] [default to undefined]
**artifactUrl** | **string** | 构建产物下载地址 | [optional] [default to undefined]
**artifactSize** | **number** | 构建产物大小 (字节) | [optional] [default to undefined]

## Example

```typescript
import { UpdateBuildRecordDto } from 'puupee-api';

const instance: UpdateBuildRecordDto = {
    status,
    logs,
    errorMessage,
    artifactUrl,
    artifactSize,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
