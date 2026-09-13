# CreateOrUpdateAiProviderDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**display_name** | **string** |  | [optional] [default to undefined]
**provider_type** | [**AiProviderType**](AiProviderType.md) |  | [optional] [default to undefined]
**base_url** | **string** |  | [optional] [default to undefined]
**region** | **string** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**capabilities** | [**Array&lt;AiCapability&gt;**](AiCapability.md) |  | [optional] [default to undefined]
**secret** | **string** |  | [optional] [default to undefined]
**clear_secret** | **boolean** |  | [optional] [default to undefined]
**metadata** | **{ [key: string]: string | undefined; }** |  | [optional] [default to undefined]
**models** | [**Array&lt;CreateOrUpdateAiModelDto&gt;**](CreateOrUpdateAiModelDto.md) |  | [optional] [default to undefined]

## Example

```typescript
import { CreateOrUpdateAiProviderDto } from 'felorx-api';

const instance: CreateOrUpdateAiProviderDto = {
    name,
    display_name,
    provider_type,
    base_url,
    region,
    enabled,
    capabilities,
    secret,
    clear_secret,
    metadata,
    models,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
