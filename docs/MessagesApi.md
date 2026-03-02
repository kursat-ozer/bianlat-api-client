# MessagesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getMessagesApiV1ConversationsConversationIdMessagesGet**](MessagesApi.md#getmessagesapiv1conversationsconversationidmessagesget) | **GET** /api/v1/conversations/{conversation_id}/messages | Get Messages |
| [**markAsReadApiV1MessagesMessageIdReadPatch**](MessagesApi.md#markasreadapiv1messagesmessageidreadpatch) | **PATCH** /api/v1/messages/{message_id}/read | Mark As Read |
| [**sendMessageApiV1ConversationsConversationIdMessagesPost**](MessagesApi.md#sendmessageapiv1conversationsconversationidmessagespost) | **POST** /api/v1/conversations/{conversation_id}/messages | Send Message |



## getMessagesApiV1ConversationsConversationIdMessagesGet

> PaginatedMessages getMessagesApiV1ConversationsConversationIdMessagesGet(conversationId, cursor, limit)

Get Messages

### Example

```ts
import {
  Configuration,
  MessagesApi,
} from '@bianlat/api-client';
import type { GetMessagesApiV1ConversationsConversationIdMessagesGetRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessagesApi(config);

  const body = {
    // string
    conversationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string (optional)
    cursor: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // number (optional)
    limit: 56,
  } satisfies GetMessagesApiV1ConversationsConversationIdMessagesGetRequest;

  try {
    const data = await api.getMessagesApiV1ConversationsConversationIdMessagesGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **conversationId** | `string` |  | [Defaults to `undefined`] |
| **cursor** | `string` |  | [Optional] [Defaults to `undefined`] |
| **limit** | `number` |  | [Optional] [Defaults to `30`] |

### Return type

[**PaginatedMessages**](PaginatedMessages.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## markAsReadApiV1MessagesMessageIdReadPatch

> markAsReadApiV1MessagesMessageIdReadPatch(messageId)

Mark As Read

### Example

```ts
import {
  Configuration,
  MessagesApi,
} from '@bianlat/api-client';
import type { MarkAsReadApiV1MessagesMessageIdReadPatchRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessagesApi(config);

  const body = {
    // string
    messageId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies MarkAsReadApiV1MessagesMessageIdReadPatchRequest;

  try {
    const data = await api.markAsReadApiV1MessagesMessageIdReadPatch(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **messageId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## sendMessageApiV1ConversationsConversationIdMessagesPost

> MessageRead sendMessageApiV1ConversationsConversationIdMessagesPost(conversationId, sendMessageRequest)

Send Message

### Example

```ts
import {
  Configuration,
  MessagesApi,
} from '@bianlat/api-client';
import type { SendMessageApiV1ConversationsConversationIdMessagesPostRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessagesApi(config);

  const body = {
    // string
    conversationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // SendMessageRequest
    sendMessageRequest: ...,
  } satisfies SendMessageApiV1ConversationsConversationIdMessagesPostRequest;

  try {
    const data = await api.sendMessageApiV1ConversationsConversationIdMessagesPost(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **conversationId** | `string` |  | [Defaults to `undefined`] |
| **sendMessageRequest** | [SendMessageRequest](SendMessageRequest.md) |  | |

### Return type

[**MessageRead**](MessageRead.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

