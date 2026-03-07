# MessagesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getMessagesApiV1ConversationsConversationIdMessagesGet**](#getmessagesapiv1conversationsconversationidmessagesget) | **GET** /api/v1/conversations/{conversation_id}/messages | Get Messages|
|[**markAsReadApiV1MessagesMessageIdReadPatch**](#markasreadapiv1messagesmessageidreadpatch) | **PATCH** /api/v1/messages/{message_id}/read | Mark As Read|
|[**markConversationAsReadApiV1ConversationsConversationIdReadPatch**](#markconversationasreadapiv1conversationsconversationidreadpatch) | **PATCH** /api/v1/conversations/{conversation_id}/read | Mark Conversation As Read|
|[**sendMessageApiV1ConversationsConversationIdMessagesPost**](#sendmessageapiv1conversationsconversationidmessagespost) | **POST** /api/v1/conversations/{conversation_id}/messages | Send Message|

# **getMessagesApiV1ConversationsConversationIdMessagesGet**
> PaginatedMessages getMessagesApiV1ConversationsConversationIdMessagesGet()


### Example

```typescript
import {
    MessagesApi,
    Configuration
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new MessagesApi(configuration);

let conversationId: string; // (default to undefined)
let cursor: string; // (optional) (default to undefined)
let limit: number; // (optional) (default to 30)

const { status, data } = await apiInstance.getMessagesApiV1ConversationsConversationIdMessagesGet(
    conversationId,
    cursor,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **conversationId** | [**string**] |  | defaults to undefined|
| **cursor** | [**string**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to 30|


### Return type

**PaginatedMessages**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **markAsReadApiV1MessagesMessageIdReadPatch**
> markAsReadApiV1MessagesMessageIdReadPatch()


### Example

```typescript
import {
    MessagesApi,
    Configuration
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new MessagesApi(configuration);

let messageId: string; // (default to undefined)

const { status, data } = await apiInstance.markAsReadApiV1MessagesMessageIdReadPatch(
    messageId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **messageId** | [**string**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **markConversationAsReadApiV1ConversationsConversationIdReadPatch**
> markConversationAsReadApiV1ConversationsConversationIdReadPatch()


### Example

```typescript
import {
    MessagesApi,
    Configuration
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new MessagesApi(configuration);

let conversationId: string; // (default to undefined)

const { status, data } = await apiInstance.markConversationAsReadApiV1ConversationsConversationIdReadPatch(
    conversationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **conversationId** | [**string**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sendMessageApiV1ConversationsConversationIdMessagesPost**
> MessageRead sendMessageApiV1ConversationsConversationIdMessagesPost(sendMessageRequest)


### Example

```typescript
import {
    MessagesApi,
    Configuration,
    SendMessageRequest
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new MessagesApi(configuration);

let conversationId: string; // (default to undefined)
let sendMessageRequest: SendMessageRequest; //

const { status, data } = await apiInstance.sendMessageApiV1ConversationsConversationIdMessagesPost(
    conversationId,
    sendMessageRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sendMessageRequest** | **SendMessageRequest**|  | |
| **conversationId** | [**string**] |  | defaults to undefined|


### Return type

**MessageRead**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

