# AppFeatureLocaleDto


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
**appFeatureId** | **string** |  | [optional] [default to undefined]
**appLocaleId** | **string** |  | [optional] [default to undefined]
**langCode** | **string** | 冗余：方便客户端展示，取自关联的 AppLocale。 | [optional] [default to undefined]
**displayName** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**details** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { AppFeatureLocaleDto } from 'puupee-api';

const instance: AppFeatureLocaleDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    appFeatureId,
    appLocaleId,
    langCode,
    displayName,
    description,
    details,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
