# ![LOGO](logo.png) Library Agent **flow**ground Connector

## Description

A generated **flow**ground connector for the Library Agent API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/libraryagent/v1/swagger.json<br/>
Generated at: 2019-05-07T17:41:45+03:00

## API Description

A simple Google Example Library API.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists shelves. The order is unspecified but deterministic. Newly created<br/>
> shelves will not necessarily be added to the end of this list.

*Tags:* `shelves`

#### Input Parameters
* `pageSize` - _optional_ - Requested page size. Server may return fewer shelves than requested.
If unspecified, server will pick an appropriate default.
* `pageToken` - _optional_ - A token identifying a page of results the server should return.
Typically, this is the value of
ListShelvesResponse.next_page_token
returned from the previous call to `ListShelves` method.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Gets a book. Returns NOT_FOUND if the book does not exist.

*Tags:* `shelves`

#### Input Parameters
* `name` - _required_ - The name of the book to retrieve.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Borrow a book from the library. Returns the book if it is borrowed<br/>
> successfully. Returns NOT_FOUND if the book does not exist in the library.<br/>
> Returns quota exceeded error if the amount of books borrowed exceeds<br/>
> allocation quota in any dimensions.

*Tags:* `shelves`

#### Input Parameters
* `name` - _required_ - The name of the book to borrow.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Return a book to the library. Returns the book if it is returned to the<br/>
> library successfully.<br/>
> Returns error if the book does not belong to the library<br/>
> or the users didn't borrow before.

*Tags:* `shelves`

#### Input Parameters
* `name` - _required_ - The name of the book to return.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists books in a shelf. The order is unspecified but deterministic. Newly<br/>
> created books will not necessarily be added to the end of this list.<br/>
> Returns NOT_FOUND if the shelf does not exist.

*Tags:* `shelves`

#### Input Parameters
* `pageSize` - _optional_ - Requested page size. Server may return fewer books than requested.
If unspecified, server will pick an appropriate default.
* `pageToken` - _optional_ - A token identifying a page of results the server should return.
Typically, this is the value of
ListBooksResponse.next_page_token.
returned from the previous call to `ListBooks` method.
* `parent` - _required_ - The name of the shelf whose books we'd like to list.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

## License

**flow**ground :- Telekom iPaaS / googleapis-com-libraryagent-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
