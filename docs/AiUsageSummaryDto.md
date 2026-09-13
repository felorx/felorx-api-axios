# AiUsageSummaryDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from** | **string** |  | [optional] [default to undefined]
**to** | **string** |  | [optional] [default to undefined]
**model_usages** | [**Array&lt;AiModelUsageDto&gt;**](AiModelUsageDto.md) |  | [optional] [default to undefined]
**runtime_usages** | **Array&lt;any&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { AiUsageSummaryDto } from 'felorx-api';

const instance: AiUsageSummaryDto = {
    from,
    to,
    model_usages,
    runtime_usages,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
