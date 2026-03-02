
# CursorPageContactRead


## Properties

Name | Type
------------ | -------------
`items` | [Array&lt;ContactRead&gt;](ContactRead.md)
`total` | number
`currentPage` | string
`currentPageBackwards` | string
`previousPage` | string
`nextPage` | string

## Example

```typescript
import type { CursorPageContactRead } from '@bianlat/api-client'

// TODO: Update the object below with actual values
const example = {
  "items": null,
  "total": null,
  "currentPage": null,
  "currentPageBackwards": null,
  "previousPage": null,
  "nextPage": null,
} satisfies CursorPageContactRead

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CursorPageContactRead
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


