# CreateBuildRecordDto

创建构建记录DTO

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appId** | **string** | 应用ID | [default to undefined]
**version** | **string** | 版本号 | [default to undefined]
**branch** | **string** | 分支名称 | [default to undefined]
**commitHash** | **string** | 提交哈希 | [default to undefined]
**trigger** | [**BuildTrigger**](BuildTrigger.md) |  | [optional] [default to undefined]
**platform** | [**AppPlatform**](AppPlatform.md) |  | [default to undefined]
**artifactType** | [**ArtifactType**](ArtifactType.md) |  | [default to undefined]
**environment** | **string** | 环境 | [optional] [default to undefined]
**ciSystem** | **string** | CI/CD 系统信息 | [optional] [default to undefined]
**ciBuildId** | **string** | CI/CD 构建ID | [optional] [default to undefined]
**ciBuildUrl** | **string** | CI/CD 构建URL | [optional] [default to undefined]

## Example

```typescript
import { CreateBuildRecordDto } from 'puupee-api';

const instance: CreateBuildRecordDto = {
    appId,
    version,
    branch,
    commitHash,
    trigger,
    platform,
    artifactType,
    environment,
    ciSystem,
    ciBuildId,
    ciBuildUrl,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
