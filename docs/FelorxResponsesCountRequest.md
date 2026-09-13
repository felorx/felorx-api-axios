# FelorxResponsesCountRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**model** | **string** |  | [optional] [default to undefined]
**input** | [**FelorxResponseInput**](FelorxResponseInput.md) |  | [optional] [default to undefined]
**instructions** | **string** |  | [optional] [default to undefined]
**previous_response_id** | **string** |  | [optional] [default to undefined]
**tools** | [**Array&lt;FelorxResponsesCountRequestToolsInner&gt;**](FelorxResponsesCountRequestToolsInner.md) |  | [optional] [default to undefined]
**tool_choice** | [**FelorxResponseToolChoice**](FelorxResponseToolChoice.md) |  | [optional] [default to undefined]
**parallel_tool_calls** | **boolean** |  | [optional] [default to undefined]
**reasoning** | **object** |  | [optional] [default to undefined]
**text** | **object** |  | [optional] [default to undefined]
**truncation** | **string** |  | [optional] [default to undefined]
**personality** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FelorxResponsesCountRequest } from 'felorx-api';

const instance: FelorxResponsesCountRequest = {
    model,
    input,
    instructions,
    previous_response_id,
    tools,
    tool_choice,
    parallel_tool_calls,
    reasoning,
    text,
    truncation,
    personality,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
