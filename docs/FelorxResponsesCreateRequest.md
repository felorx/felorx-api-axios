# FelorxResponsesCreateRequest

Only function/custom tool declarations are supported. Provider-managed conversation, prompt, item and file references are rejected. Inline input content is supported. Background requests require storage.

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
**stream** | **boolean** |  | [optional] [default to undefined]
**store** | **boolean** |  | [optional] [default to undefined]
**background** | **boolean** |  | [optional] [default to undefined]
**max_output_tokens** | **number** |  | [optional] [default to undefined]
**temperature** | **number** |  | [optional] [default to undefined]
**top_p** | **number** |  | [optional] [default to undefined]
**metadata** | **object** |  | [optional] [default to undefined]
**service_tier** | **string** |  | [optional] [default to undefined]
**prompt_cache_key** | **string** |  | [optional] [default to undefined]
**prompt_cache_retention** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { FelorxResponsesCreateRequest } from 'felorx-api';

const instance: FelorxResponsesCreateRequest = {
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
    stream,
    store,
    background,
    max_output_tokens,
    temperature,
    top_p,
    metadata,
    service_tier,
    prompt_cache_key,
    prompt_cache_retention,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
