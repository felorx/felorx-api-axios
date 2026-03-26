# DeviceDto


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
**token** | **string** |  | [optional] [default to undefined]
**isPhysicalDevice** | **boolean** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**platform** | [**AppPlatform**](AppPlatform.md) |  | [optional] [default to undefined]
**brand** | **string** |  | [optional] [default to undefined]
**systemVersion** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { DeviceDto } from 'puupee-api';

const instance: DeviceDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    token,
    isPhysicalDevice,
    name,
    platform,
    brand,
    systemVersion,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
