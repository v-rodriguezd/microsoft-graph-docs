List conversationMembers
Namespace: microsoft.graph
[!INCLUDE v1.0 disclaimer]
List all conversation members in a chat or channel.
Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.
Permission Type | Permissions (from least to most privileged)
--------------- | ----------------
Delegated (work or school account) | Chat.ReadBasic, Chat.Read, Chat.ReadWrite
Delegated (personal Microsoft account) | Not supported.
Application | Not supported.
[!NOTE] Before calling this API with application permissions, you must request access. For details, see Protected APIs in Microsoft Teams.
HTTP request (as per instructions not to include getchat)
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
Optional query parameters
This operation does not support the OData Query Parameters to customize the response.
Request headers
Header | Value
------ | ------
Authorization | Bearer {token}. Required.
Request body
Do not supply a request body for this method.

Response
If successful, this method returns a 200 OK response code and a list of conversationMember objects in the response body.
Example
Request
Here is an example of the request.

HTTP
GET https://graph.microsoft.com/v1.0/me/chats/{id}/members
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "roles": [],
            "displayName": "John Doe",
            "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "email": null
        }
    ]
}
