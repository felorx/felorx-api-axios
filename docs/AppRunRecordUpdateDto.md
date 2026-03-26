# AppRunRecordUpdateDto


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
**status** | [**AppRunStatus**](AppRunStatus.md) |  | [default to undefined]
**result** | **string** |  | [optional] [default to undefined]
**error** | **string** |  | [optional] [default to undefined]
**finishAt** | **string** |  | [optional] [default to undefined]
**output** | **string** |  | [optional] [default to undefined]
**workerId** | **string** |  | [default to undefined]
**workerName** | **string** |  | [default to undefined]

## Example

```typescript
import { AppRunRecordUpdateDto } from 'puupee-api';

const instance: AppRunRecordUpdateDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
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
