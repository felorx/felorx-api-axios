# DeployRecordDto

部署记录DTO

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
**buildRecordId** | **string** | 构建记录ID | [optional] [default to undefined]
**buildRecordVersion** | **string** | 构建记录版本 | [optional] [default to undefined]
**version** | **string** | 版本号 | [optional] [default to undefined]
**platform** | [**AppPlatform**](AppPlatform.md) |  | [optional] [default to undefined]
**environment** | **string** | 部署环境 | [optional] [default to undefined]
**status** | [**DeployStatus**](DeployStatus.md) |  | [optional] [default to undefined]
**startedAt** | **string** | 开始时间 | [optional] [default to undefined]
**completedAt** | **string** | 结束时间 | [optional] [default to undefined]
**errorMessage** | **string** | 错误信息 | [optional] [default to undefined]
**deployUrl** | **string** | 部署地址 | [optional] [default to undefined]
**deployTarget** | **string** | 部署目标 | [optional] [default to undefined]
**deployChannel** | **string** | 部署渠道 | [optional] [default to undefined]
**ciSystem** | **string** | CI/CD 系统信息 | [optional] [default to undefined]
**ciDeployId** | **string** | CI/CD 部署ID | [optional] [default to undefined]
**ciDeployUrl** | **string** | CI/CD 部署URL | [optional] [default to undefined]
**duration** | **number** | 部署持续时间 (秒) | [optional] [default to undefined]

## Example

```typescript
import { DeployRecordDto } from 'puupee-api';

const instance: DeployRecordDto = {
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
    buildRecordId,
    buildRecordVersion,
    version,
    platform,
    environment,
    status,
    startedAt,
    completedAt,
    errorMessage,
    deployUrl,
    deployTarget,
    deployChannel,
    ciSystem,
    ciDeployId,
    ciDeployUrl,
    duration,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
