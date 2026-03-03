# ConversationRead


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**type** | [**ConversationType**](ConversationType.md) |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**avatar** | **string** |  | [default to undefined]
**participants** | [**Array&lt;ParticipantRead&gt;**](ParticipantRead.md) |  | [default to undefined]
**last_message** | [**LastMessageRead**](LastMessageRead.md) |  | [default to undefined]
**unread_count** | **number** |  | [default to undefined]
**created_at** | **string** |  | [default to undefined]
**updated_at** | **string** |  | [default to undefined]

## Example

```typescript
import { ConversationRead } from '@bianlat/api-client';

const instance: ConversationRead = {
    id,
    type,
    name,
    avatar,
    participants,
    last_message,
    unread_count,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
