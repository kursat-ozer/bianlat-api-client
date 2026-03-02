
# ParticipantRead


## Properties

Name | Type
------------ | -------------
`userId` | string
`role` | [ParticipantRole](ParticipantRole.md)
`unreadCount` | number
`joinedAt` | Date

## Example

```typescript
import type { ParticipantRead } from '@bianlat/api-client'

// TODO: Update the object below with actual values
const example = {
  "userId": null,
  "role": null,
  "unreadCount": null,
  "joinedAt": null,
} satisfies ParticipantRead

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ParticipantRead
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


