# ControllerApiDescriptionModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**controllerName** | **string** |  | [optional] [default to undefined]
**controllerGroupName** | **string** |  | [optional] [default to undefined]
**isRemoteService** | **boolean** |  | [optional] [default to undefined]
**isIntegrationService** | **boolean** |  | [optional] [default to undefined]
**apiVersion** | **string** |  | [optional] [default to undefined]
**type** | **string** |  | [optional] [default to undefined]
**interfaces** | [**Array&lt;ControllerInterfaceApiDescriptionModel&gt;**](ControllerInterfaceApiDescriptionModel.md) |  | [optional] [default to undefined]
**actions** | [**{ [key: string]: ActionApiDescriptionModel | undefined; }**](ActionApiDescriptionModel.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ControllerApiDescriptionModel } from 'puupee-api';

const instance: ControllerApiDescriptionModel = {
    controllerName,
    controllerGroupName,
    isRemoteService,
    isIntegrationService,
    apiVersion,
    type,
    interfaces,
    actions,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
