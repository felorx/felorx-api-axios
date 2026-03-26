# TypeApiDescriptionModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**baseType** | **string** |  | [optional] [default to undefined]
**isEnum** | **boolean** |  | [optional] [default to undefined]
**enumNames** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**enumValues** | **Array&lt;any&gt;** |  | [optional] [default to undefined]
**genericArguments** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**properties** | [**Array&lt;PropertyApiDescriptionModel&gt;**](PropertyApiDescriptionModel.md) |  | [optional] [default to undefined]

## Example

```typescript
import { TypeApiDescriptionModel } from 'puupee-api';

const instance: TypeApiDescriptionModel = {
    baseType,
    isEnum,
    enumNames,
    enumValues,
    genericArguments,
    properties,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
