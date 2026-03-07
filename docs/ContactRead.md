# ContactRead

Hem aktif (kayıtlı) hem de pending (kayıtsız) kişileri temsil eder.  id      → her zaman UserContact.id (PATCH/DELETE /contacts/{id} için kullanılır) user_id → sadece aktif contact\'larda User UUID\'si (sohbet başlatmak için); pending\'de None first_name is None → kişi henüz uygulamaya kayıt olmamış (pending)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**user_id** | **string** |  | [optional] [default to undefined]
**phone** | **string** |  | [default to undefined]
**first_name** | **string** |  | [optional] [default to undefined]
**last_name** | **string** |  | [optional] [default to undefined]
**bio** | **string** |  | [optional] [default to undefined]
**is_active** | **boolean** |  | [optional] [default to false]
**created_at** | **string** |  | [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { ContactRead } from '@bianlat/api-client';

const instance: ContactRead = {
    id,
    user_id,
    phone,
    first_name,
    last_name,
    bio,
    is_active,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
