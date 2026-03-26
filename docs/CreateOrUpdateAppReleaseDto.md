# CreateOrUpdateAppReleaseDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **string** |  | [optional] [default to undefined]
**versionName** | **string** | 版本名称 | [optional] [default to undefined]
**versionCode** | **number** | 构建编号 | [optional] [default to undefined]
**notes** | **string** |  | [optional] [default to undefined]
**platform** | [**AppPlatform**](AppPlatform.md) |  | [optional] [default to undefined]
**key** | **string** |  | [optional] [default to undefined]
**rapidCode** | **string** |  | [optional] [default to undefined]
**size** | **number** |  | [optional] [default to undefined]
**hash** | **string** |  | [optional] [default to undefined]
**artifactType** | [**ArtifactType**](ArtifactType.md) |  | [optional] [default to undefined]
**publisher** | [**AppPublisher**](AppPublisher.md) |  | [optional] [default to undefined]
**isForceUpdate** | **boolean** |  | [optional] [default to undefined]
**appId** | **string** |  | [optional] [default to undefined]
**isEnabled** | **boolean** |  | [optional] [default to undefined]
**channel** | [**ReleaseChannel**](ReleaseChannel.md) |  | [optional] [default to undefined]
**buildRecordId** | **string** | 构建记录ID（可选，如果提供则使用对应构建的BuildNumber作为VersionCode） | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateAppReleaseDto } from 'puupee-api';

const instance: CreateOrUpdateAppReleaseDto = {
    version,
    versionName,
    versionCode,
    notes,
    platform,
    key,
    rapidCode,
    size,
    hash,
    artifactType,
    publisher,
    isForceUpdate,
    appId,
    isEnabled,
    channel,
    buildRecordId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
