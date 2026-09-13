# AiModelDto


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
**verified_capabilities** | [**Array&lt;AiCapability&gt;**](AiCapability.md) |  | [optional] [default to undefined]
**capability_certificate_version** | **string** |  | [optional] [default to undefined]
**capability_tested_at** | **string** |  | [optional] [default to undefined]
**provider_id** | **string** |  | [optional] [default to undefined]
**route_name** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**display_name** | **string** |  | [optional] [default to undefined]
**capabilities** | [**Array&lt;AiCapability&gt;**](AiCapability.md) |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**is_default** | **boolean** |  | [optional] [default to undefined]
**default_parameters** | **{ [key: string]: string | undefined; }** |  | [optional] [default to undefined]

## Example

```typescript
import { AiModelDto } from 'felorx-api';

const instance: AiModelDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    verified_capabilities,
    capability_certificate_version,
    capability_tested_at,
    provider_id,
    route_name,
    name,
    display_name,
    capabilities,
    enabled,
    is_default,
    default_parameters,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
