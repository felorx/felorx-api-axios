# CreateOrUpdateAiModelDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**route_name** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**display_name** | **string** |  | [optional] [default to undefined]
**capabilities** | [**Array&lt;AiCapability&gt;**](AiCapability.md) |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**is_default** | **boolean** |  | [optional] [default to undefined]
**default_parameters** | **{ [key: string]: string | undefined; }** |  | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateAiModelDto } from 'felorx-api';

const instance: CreateOrUpdateAiModelDto = {
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
