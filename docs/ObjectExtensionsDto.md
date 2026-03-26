# ObjectExtensionsDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**modules** | [**{ [key: string]: ModuleExtensionDto | undefined; }**](ModuleExtensionDto.md) |  | [optional] [default to undefined]
**enums** | [**{ [key: string]: ExtensionEnumDto | undefined; }**](ExtensionEnumDto.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ObjectExtensionsDto } from 'puupee-api';

const instance: ObjectExtensionsDto = {
    modules,
    enums,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
