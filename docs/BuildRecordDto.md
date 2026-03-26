# BuildRecordDto

构建记录DTO

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
**version** | **string** | 版本号 | [optional] [default to undefined]
**branch** | **string** | 分支名称 | [optional] [default to undefined]
**commitHash** | **string** | 提交哈希 | [optional] [default to undefined]
**trigger** | [**BuildTrigger**](BuildTrigger.md) |  | [optional] [default to undefined]
**platform** | [**AppPlatform**](AppPlatform.md) |  | [optional] [default to undefined]
**artifactType** | [**ArtifactType**](ArtifactType.md) |  | [optional] [default to undefined]
**environment** | **string** | 环境 | [optional] [default to undefined]
**buildNumber** | **number** | 构建号 | [optional] [default to undefined]
**status** | [**BuildStatus**](BuildStatus.md) |  | [optional] [default to undefined]
**startedAt** | **string** | 开始时间 | [optional] [default to undefined]
**completedAt** | **string** | 结束时间 | [optional] [default to undefined]
**errorMessage** | **string** | 错误信息 | [optional] [default to undefined]
**artifactUrl** | **string** | 构建产物下载地址 | [optional] [default to undefined]
**artifactSize** | **number** | 构建产物大小 (字节) | [optional] [default to undefined]
**ciSystem** | **string** | CI/CD 系统信息 | [optional] [default to undefined]
**ciBuildId** | **string** | CI/CD 构建ID | [optional] [default to undefined]
**ciBuildUrl** | **string** | CI/CD 构建URL | [optional] [default to undefined]
**duration** | **number** | 构建持续时间 (秒) | [optional] [default to undefined]

## Example

```typescript
import { BuildRecordDto } from 'puupee-api';

const instance: BuildRecordDto = {
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
    version,
    branch,
    commitHash,
    trigger,
    platform,
    artifactType,
    environment,
    buildNumber,
    status,
    startedAt,
    completedAt,
    errorMessage,
    artifactUrl,
    artifactSize,
    ciSystem,
    ciBuildId,
    ciBuildUrl,
    duration,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
