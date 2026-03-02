
# LastMessageRead


## Properties

Name | Type
------------ | -------------
`id` | string
`conversationId` | string
`senderId` | string
`messageType` | [MessageType](MessageType.md)
`content` | string
`status` | [MessageStatus](MessageStatus.md)
`createdAt` | Date

## Example

```typescript
import type { LastMessageRead } from '@bianlat/api-client'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "conversationId": null,
  "senderId": null,
  "messageType": null,
  "content": null,
  "status": null,
  "createdAt": null,
} satisfies LastMessageRead

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LastMessageRead
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


