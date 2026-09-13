# OpenAiChatCompletionRequestDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**model** | **string** |  | [optional] [default to undefined]
**provider** | **string** |  | [optional] [default to undefined]
**messages** | [**Array&lt;AiChatMessageDto&gt;**](AiChatMessageDto.md) |  | [optional] [default to undefined]
**temperature** | **number** |  | [optional] [default to undefined]
**top_p** | **number** |  | [optional] [default to undefined]
**max_tokens** | **number** |  | [optional] [default to undefined]
**stream** | **boolean** |  | [optional] [default to undefined]
**metadata** | **{ [key: string]: string | undefined; }** |  | [optional] [default to undefined]

## Example

```typescript
import { OpenAiChatCompletionRequestDto } from 'felorx-api';

const instance: OpenAiChatCompletionRequestDto = {
    model,
    provider,
    messages,
    temperature,
    top_p,
    max_tokens,
    stream,
    metadata,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
