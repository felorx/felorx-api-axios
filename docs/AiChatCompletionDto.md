# AiChatCompletionDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**object** | **string** |  | [optional] [default to undefined]
**created** | **number** |  | [optional] [default to undefined]
**model** | **string** |  | [optional] [default to undefined]
**choices** | [**Array&lt;AiChatChoiceDto&gt;**](AiChatChoiceDto.md) |  | [optional] [default to undefined]
**usage** | [**AiUsageDto**](AiUsageDto.md) |  | [optional] [default to undefined]

## Example

```typescript
import { AiChatCompletionDto } from 'felorx-api';

const instance: AiChatCompletionDto = {
    id,
    object,
    created,
    model,
    choices,
    usage,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
