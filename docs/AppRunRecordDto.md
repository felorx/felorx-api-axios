# AppRunRecordDto


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
**appId** | **string** |  | [optional] [default to undefined]
**appName** | **string** |  | [optional] [default to undefined]
**args** | **any** |  | [optional] [default to undefined]
**envs** | **any** |  | [optional] [default to undefined]
**status** | [**AppRunStatus**](AppRunStatus.md) |  | [optional] [default to undefined]
**result** | **string** |  | [optional] [default to undefined]
**error** | **string** |  | [optional] [default to undefined]
**finishAt** | **string** |  | [optional] [default to undefined]
**output** | **string** |  | [optional] [default to undefined]
**workerId** | **string** |  | [optional] [default to undefined]
**workerName** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { AppRunRecordDto } from 'puupee-api';

const instance: AppRunRecordDto = {
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
    args,
    envs,
    status,
    result,
    error,
    finishAt,
    output,
    workerId,
    workerName,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
