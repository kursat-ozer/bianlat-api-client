
# ConversationCreate


## Properties

Name | Type
------------ | -------------
`participantIds` | Array&lt;string&gt;
`type` | [ConversationType](ConversationType.md)
`name` | string

## Example

```typescript
import type { ConversationCreate } from '@bianlat/api-client'

// TODO: Update the object below with actual values
const example = {
  "participantIds": null,
  "type": null,
  "name": null,
} satisfies ConversationCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ConversationCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


