# AppPricingItemValueDto


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
**isAvailable** | **boolean** | 是否可用 | [optional] [default to undefined]
**hasValue** | **boolean** | 是否有值 | [optional] [default to undefined]
**intValue** | **number** |  | [optional] [default to undefined]
**stringValue** | **string** |  | [optional] [default to undefined]
**boolValue** | **boolean** |  | [optional] [default to undefined]
**intValueType** | **string** | 数字值类型, FileSize: 文件大小, Count: 数目 | [optional] [default to undefined]

## Example

```typescript
import { AppPricingItemValueDto } from 'puupee-api';

const instance: AppPricingItemValueDto = {
    id,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    isAvailable,
    hasValue,
    intValue,
    stringValue,
    boolValue,
    intValueType,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
