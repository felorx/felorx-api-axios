# CreateDeployRecordDto

创建部署记录DTO

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appId** | **string** | 应用ID | [default to undefined]
**buildRecordId** | **string** | 构建记录ID | [default to undefined]
**version** | **string** | 版本号 | [default to undefined]
**platform** | [**AppPlatform**](AppPlatform.md) |  | [default to undefined]
**environment** | **string** | 部署环境 | [default to undefined]
**deployUrl** | **string** | 部署地址 | [optional] [default to undefined]
**deployTarget** | **string** | 部署目标 | [optional] [default to undefined]
**deployChannel** | **string** | 部署渠道 | [optional] [default to undefined]
**ciSystem** | **string** | CI/CD 系统信息 | [optional] [default to undefined]
**ciDeployId** | **string** | CI/CD 部署ID | [optional] [default to undefined]
**ciDeployUrl** | **string** | CI/CD 部署URL | [optional] [default to undefined]

## Example

```typescript
import { CreateDeployRecordDto } from 'puupee-api';

const instance: CreateDeployRecordDto = {
    appId,
    buildRecordId,
    version,
    platform,
    environment,
    deployUrl,
    deployTarget,
    deployChannel,
    ciSystem,
    ciDeployId,
    ciDeployUrl,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
