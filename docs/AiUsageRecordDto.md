# AiUsageRecordDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**logical_model** | **string** |  | [optional] [default to undefined]
**model_charge_kind** | **string** |  | [optional] [default to undefined]
**runtime_charge_kind** | **string** |  | [optional] [default to undefined]
**input_tokens** | **number** |  | [optional] [default to undefined]
**output_tokens** | **number** |  | [optional] [default to undefined]
**total_tokens** | **number** |  | [optional] [default to undefined]
**runtime_milliseconds** | **number** |  | [optional] [default to undefined]
**observed_at** | **string** |  | [optional] [default to undefined]
**estimated_model_cost_microusd** | **number** |  | [optional] [default to undefined]
**estimated_runtime_cost_microusd** | **number** |  | [optional] [default to undefined]
**pricing_effective_at** | **string** |  | [optional] [default to undefined]
**pricing_captured_at** | **string** |  | [optional] [default to undefined]
**pricing_source_url** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { AiUsageRecordDto } from 'felorx-api';

const instance: AiUsageRecordDto = {
    id,
    logical_model,
    model_charge_kind,
    runtime_charge_kind,
    input_tokens,
    output_tokens,
    total_tokens,
    runtime_milliseconds,
    observed_at,
    estimated_model_cost_microusd,
    estimated_runtime_cost_microusd,
    pricing_effective_at,
    pricing_captured_at,
    pricing_source_url,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
