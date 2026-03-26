# UpdateDeployRecordDto

更新部署记录DTO

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | [**DeployStatus**](DeployStatus.md) |  | [default to undefined]
**logs** | **string** | 部署日志 | [optional] [default to undefined]
**errorMessage** | **string** | 错误信息 | [optional] [default to undefined]
**deployUrl** | **string** | 部署地址 | [optional] [default to undefined]

## Example

```typescript
import { UpdateDeployRecordDto } from 'puupee-api';

const instance: UpdateDeployRecordDto = {
    status,
    logs,
    errorMessage,
    deployUrl,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
