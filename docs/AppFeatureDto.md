# AppFeatureDto


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
**appId** | **string** | 所属应用ID | [optional] [default to undefined]
**name** | **string** | 功能名称（唯一标识，同一应用内唯一） | [optional] [default to undefined]
**sort** | **number** |  | [optional] [default to undefined]
**featureLocales** | [**Array&lt;AppFeatureLocaleDto&gt;**](AppFeatureLocaleDto.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AppFeatureDto } from 'puupee-api';

const instance: AppFeatureDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    appId,
    name,
    sort,
    featureLocales,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
