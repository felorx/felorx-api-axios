# ExtensionPropertyDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **string** |  | [optional] [default to undefined]
**typeSimple** | **string** |  | [optional] [default to undefined]
**displayName** | [**LocalizableStringDto**](LocalizableStringDto.md) |  | [optional] [default to undefined]
**api** | [**ExtensionPropertyApiDto**](ExtensionPropertyApiDto.md) |  | [optional] [default to undefined]
**ui** | [**ExtensionPropertyUiDto**](ExtensionPropertyUiDto.md) |  | [optional] [default to undefined]
**attributes** | [**Array&lt;ExtensionPropertyAttributeDto&gt;**](ExtensionPropertyAttributeDto.md) |  | [optional] [default to undefined]
**configuration** | **{ [key: string]: any | undefined; }** |  | [optional] [default to undefined]
**defaultValue** | **any** |  | [optional] [default to undefined]

## Example

```typescript
import { ExtensionPropertyDto } from 'puupee-api';

const instance: ExtensionPropertyDto = {
    type,
    typeSimple,
    displayName,
    api,
    ui,
    attributes,
    configuration,
    defaultValue,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
