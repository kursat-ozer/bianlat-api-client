
# ConversationRead


## Properties

Name | Type
------------ | -------------
`id` | string
`type` | [ConversationType](ConversationType.md)
`name` | string
`avatar` | string
`participants` | [Array&lt;ParticipantRead&gt;](ParticipantRead.md)
`lastMessage` | [LastMessageRead](LastMessageRead.md)
`unreadCount` | number
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { ConversationRead } from '@bianlat/api-client'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "type": null,
  "name": null,
  "avatar": null,
  "participants": null,
  "lastMessage": null,
  "unreadCount": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies ConversationRead

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ConversationRead
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


