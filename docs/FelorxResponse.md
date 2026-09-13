# FelorxResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**object** | **string** |  | [default to undefined]
**model** | **string** |  | [optional] [default to undefined]
**status** | **string** |  | [default to undefined]
**output** | **Array&lt;object&gt;** |  | [default to undefined]
**created_at** | **number** |  | [optional] [default to undefined]
**previous_response_id** | **string** |  | [optional] [default to undefined]
**usage** | [**FelorxResponseUsage**](FelorxResponseUsage.md) |  | [optional] [default to undefined]
**error** | **object** |  | [optional] [default to undefined]
**incomplete_details** | **object** |  | [optional] [default to undefined]

## Example

```typescript
import { FelorxResponse } from 'felorx-api';

const instance: FelorxResponse = {
    id,
    object,
    model,
    status,
    output,
    created_at,
    previous_response_id,
    usage,
    error,
    incomplete_details,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
