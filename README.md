## @bianlat/api-client@0.1.2

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install @bianlat/api-client@0.1.2 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *http://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AuthApi* | [**loginApiV1AuthLoginPost**](docs/AuthApi.md#loginapiv1authloginpost) | **POST** /api/v1/auth/login | Login
*AuthApi* | [**logoutApiV1AuthLogoutPost**](docs/AuthApi.md#logoutapiv1authlogoutpost) | **POST** /api/v1/auth/logout | Logout
*AuthApi* | [**refreshApiV1AuthRefreshPost**](docs/AuthApi.md#refreshapiv1authrefreshpost) | **POST** /api/v1/auth/refresh | Refresh
*AuthApi* | [**verifyApiV1AuthVerifyPost**](docs/AuthApi.md#verifyapiv1authverifypost) | **POST** /api/v1/auth/verify | Verify
*ConversationsApi* | [**createConversationApiV1ConversationsPost**](docs/ConversationsApi.md#createconversationapiv1conversationspost) | **POST** /api/v1/conversations | Create Conversation
*ConversationsApi* | [**deleteConversationApiV1ConversationsConversationIdDelete**](docs/ConversationsApi.md#deleteconversationapiv1conversationsconversationiddelete) | **DELETE** /api/v1/conversations/{conversation_id} | Delete Conversation
*ConversationsApi* | [**getConversationApiV1ConversationsConversationIdGet**](docs/ConversationsApi.md#getconversationapiv1conversationsconversationidget) | **GET** /api/v1/conversations/{conversation_id} | Get Conversation
*ConversationsApi* | [**listConversationsApiV1ConversationsGet**](docs/ConversationsApi.md#listconversationsapiv1conversationsget) | **GET** /api/v1/conversations | List Conversations
*HealthApi* | [**healthHealthGet**](docs/HealthApi.md#healthhealthget) | **GET** /health | Health
*MessagesApi* | [**getMessagesApiV1ConversationsConversationIdMessagesGet**](docs/MessagesApi.md#getmessagesapiv1conversationsconversationidmessagesget) | **GET** /api/v1/conversations/{conversation_id}/messages | Get Messages
*MessagesApi* | [**markAsReadApiV1MessagesMessageIdReadPatch**](docs/MessagesApi.md#markasreadapiv1messagesmessageidreadpatch) | **PATCH** /api/v1/messages/{message_id}/read | Mark As Read
*MessagesApi* | [**markConversationAsReadApiV1ConversationsConversationIdReadPatch**](docs/MessagesApi.md#markconversationasreadapiv1conversationsconversationidreadpatch) | **PATCH** /api/v1/conversations/{conversation_id}/read | Mark Conversation As Read
*MessagesApi* | [**sendMessageApiV1ConversationsConversationIdMessagesPost**](docs/MessagesApi.md#sendmessageapiv1conversationsconversationidmessagespost) | **POST** /api/v1/conversations/{conversation_id}/messages | Send Message
*UsersApi* | [**addContactApiV1UsersContactsPost**](docs/UsersApi.md#addcontactapiv1userscontactspost) | **POST** /api/v1/users/contacts | Add Contact
*UsersApi* | [**getContactApiV1UsersContactsContactUserIdGet**](docs/UsersApi.md#getcontactapiv1userscontactscontactuseridget) | **GET** /api/v1/users/contacts/{contact_user_id} | Get Contact
*UsersApi* | [**getMeApiV1UsersMeGet**](docs/UsersApi.md#getmeapiv1usersmeget) | **GET** /api/v1/users/me | Get Me
*UsersApi* | [**listContactsApiV1UsersContactsGet**](docs/UsersApi.md#listcontactsapiv1userscontactsget) | **GET** /api/v1/users/contacts | List Contacts
*UsersApi* | [**removeContactApiV1UsersContactsContactIdDelete**](docs/UsersApi.md#removecontactapiv1userscontactscontactiddelete) | **DELETE** /api/v1/users/contacts/{contact_id} | Remove Contact
*UsersApi* | [**updateContactApiV1UsersContactsContactIdPatch**](docs/UsersApi.md#updatecontactapiv1userscontactscontactidpatch) | **PATCH** /api/v1/users/contacts/{contact_id} | Update Contact
*UsersApi* | [**updateMeApiV1UsersMePatch**](docs/UsersApi.md#updatemeapiv1usersmepatch) | **PATCH** /api/v1/users/me | Update Me


### Documentation For Models

 - [ContactAddResult](docs/ContactAddResult.md)
 - [ContactCreate](docs/ContactCreate.md)
 - [ContactRead](docs/ContactRead.md)
 - [ContactUpdate](docs/ContactUpdate.md)
 - [ConversationCreate](docs/ConversationCreate.md)
 - [ConversationRead](docs/ConversationRead.md)
 - [ConversationType](docs/ConversationType.md)
 - [CursorPageContactRead](docs/CursorPageContactRead.md)
 - [CursorPageConversationRead](docs/CursorPageConversationRead.md)
 - [HTTPValidationError](docs/HTTPValidationError.md)
 - [HealthResponse](docs/HealthResponse.md)
 - [LastMessageRead](docs/LastMessageRead.md)
 - [LocationInner](docs/LocationInner.md)
 - [LoginRequest](docs/LoginRequest.md)
 - [MessageRead](docs/MessageRead.md)
 - [MessageStatus](docs/MessageStatus.md)
 - [MessageType](docs/MessageType.md)
 - [PaginatedMessages](docs/PaginatedMessages.md)
 - [ParticipantRead](docs/ParticipantRead.md)
 - [ParticipantRole](docs/ParticipantRole.md)
 - [RefreshRequest](docs/RefreshRequest.md)
 - [SendMessageRequest](docs/SendMessageRequest.md)
 - [TokenResponse](docs/TokenResponse.md)
 - [UserRead](docs/UserRead.md)
 - [UserUpdate](docs/UserUpdate.md)
 - [ValidationError](docs/ValidationError.md)
 - [VerifyRequest](docs/VerifyRequest.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="HTTPBearer"></a>
### HTTPBearer

- **Type**: Bearer authentication

