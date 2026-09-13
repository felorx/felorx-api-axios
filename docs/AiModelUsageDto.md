# AiModelUsageDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**charge_kind** | **string** |  | [optional] [default to undefined]
**request_count** | **number** |  | [optional] [default to undefined]
**input_tokens** | **number** |  | [optional] [default to undefined]
**cached_input_tokens** | **number** |  | [optional] [default to undefined]
**output_tokens** | **number** |  | [optional] [default to undefined]
**reasoning_tokens** | **number** |  | [optional] [default to undefined]
**total_tokens** | **number** |  | [optional] [default to undefined]
**priced_request_count** | **number** |  | [optional] [default to undefined]
**unpriced_request_count** | **number** |  | [optional] [default to undefined]
**estimated_cost_microusd** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { AiModelUsageDto } from 'felorx-api';

const instance: AiModelUsageDto = {
    charge_kind,
    request_count,
    input_tokens,
    cached_input_tokens,
    output_tokens,
    reasoning_tokens,
    total_tokens,
    priced_request_count,
    unpriced_request_count,
    estimated_cost_microusd,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
