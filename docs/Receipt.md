# Receipt


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**receipt_type** | **string** |  | [optional] [default to undefined]
**adam_id** | **number** |  | [optional] [default to undefined]
**app_item_id** | **number** |  | [optional] [default to undefined]
**bundle_id** | **string** |  | [optional] [default to undefined]
**application_version** | **string** |  | [optional] [default to undefined]
**download_id** | **number** |  | [optional] [default to undefined]
**version_external_identifier** | **number** |  | [optional] [default to undefined]
**receipt_creation_date** | **string** |  | [optional] [default to undefined]
**receipt_creation_date_ms** | **string** |  | [optional] [default to undefined]
**receipt_creation_date_pst** | **string** |  | [optional] [default to undefined]
**request_date** | **string** |  | [optional] [default to undefined]
**request_date_ms** | **string** |  | [optional] [default to undefined]
**request_date_pst** | **string** |  | [optional] [default to undefined]
**original_purchase_date** | **string** |  | [optional] [default to undefined]
**original_purchase_date_ms** | **string** |  | [optional] [default to undefined]
**original_purchase_date_pst** | **string** |  | [optional] [default to undefined]
**original_application_version** | **string** |  | [optional] [default to undefined]
**in_app** | [**Array&lt;InApp&gt;**](InApp.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Receipt } from 'puupee-api';

const instance: Receipt = {
    receipt_type,
    adam_id,
    app_item_id,
    bundle_id,
    application_version,
    download_id,
    version_external_identifier,
    receipt_creation_date,
    receipt_creation_date_ms,
    receipt_creation_date_pst,
    request_date,
    request_date_ms,
    request_date_pst,
    original_purchase_date,
    original_purchase_date_ms,
    original_purchase_date_pst,
    original_application_version,
    in_app,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
