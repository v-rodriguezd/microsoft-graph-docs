Get conversationMember

Namespace: microsoft.graph

[!INCLUDE v1.0-disclaimer]

Retrieve a conversationMember from a chat or channel.

Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.

Permission Type	| Permissions (from least to most privileged)
--------------- | ---------------
Delegated (work or school account)	| For user or chat resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite For channel resource: ChannelMember.Read.All, ChannelMember.ReadWrite, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All
Delegated (personal Microsoft account)	| Not supported.
Application	| For user or chat resource: Not supported. For channel resource: Member.Read.Group*, ChannelMember.Read.All, ChannelMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All
Note: Permissions marked with * use resource-specific consent.

[!NOTE] Before calling this API with application permissions, you must request access. For details, see Protected APIs in Microsoft Teams.

HTTP request
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
Optional query parameters
This operation does not support the OData query parameters to customize the response.

Request headers
Header	| Value
------- | -------
Authorization	| Bearer {token}. Required.
Request body
Do not supply a request body for this method.

Response
If successful, this method returns a 200 OK response code and a conversationMember object in the response body.

Example
Request
Here is an example of the request.

HTTP
GET https://graph.microsoft.com/v1.0/chats/{id}/members/{id}
C#
[!INCLUDE sample-code] [!INCLUDE sdk-documentation]

JavaScript
[!INCLUDE sample-code] [!INCLUDE sdk-documentation]

Objective-C
[!INCLUDE sample-code] [!INCLUDE sdk-documentation]

Response
Here is an example of the response.

Note: The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "display-name-value"
}
