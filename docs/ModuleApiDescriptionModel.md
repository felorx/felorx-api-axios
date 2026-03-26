# ModuleApiDescriptionModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rootPath** | **string** |  | [optional] [default to undefined]
**remoteServiceName** | **string** |  | [optional] [default to undefined]
**controllers** | [**{ [key: string]: ControllerApiDescriptionModel | undefined; }**](ControllerApiDescriptionModel.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ModuleApiDescriptionModel } from 'puupee-api';

const instance: ModuleApiDescriptionModel = {
    rootPath,
    remoteServiceName,
    controllers,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
