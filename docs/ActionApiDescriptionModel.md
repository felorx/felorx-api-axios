# ActionApiDescriptionModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**uniqueName** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**httpMethod** | **string** |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**supportedVersions** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**parametersOnMethod** | [**Array&lt;MethodParameterApiDescriptionModel&gt;**](MethodParameterApiDescriptionModel.md) |  | [optional] [default to undefined]
**parameters** | [**Array&lt;ParameterApiDescriptionModel&gt;**](ParameterApiDescriptionModel.md) |  | [optional] [default to undefined]
**returnValue** | [**ReturnValueApiDescriptionModel**](ReturnValueApiDescriptionModel.md) |  | [optional] [default to undefined]
**allowAnonymous** | **boolean** |  | [optional] [default to undefined]
**implementFrom** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { ActionApiDescriptionModel } from 'puupee-api';

const instance: ActionApiDescriptionModel = {
    uniqueName,
    name,
    httpMethod,
    url,
    supportedVersions,
    parametersOnMethod,
    parameters,
    returnValue,
    allowAnonymous,
    implementFrom,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
