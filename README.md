# ![LOGO](logo.png) www.zoomconnect.com **flow**ground Connector

## Description

A generated **flow**ground connector for the www.zoomconnect.com API (version 1).

Generated from: https://api.apis.guru/v2/specs/zoomconnect.com/1/swagger.json<br/>
Generated at: 2019-05-07T17:45:09+03:00

## API Description

The world's greatest SMS API

## Authorization

Supported authorization schemes:
- API Key- API Key
## Actions

### balance

> Returns your account's credit balance

*Tags:* `account`

### statistics

> Returns data from the statistics report. Note that by default the statistics shown are based on the number of messages, use the calculateCreditValue should you wish to calculate the statistics based on credit value.

*Tags:* `account`

#### Input Parameters
* `from` - _optional_ - date format: dd-MM-yyyy
* `to` - _optional_ - date format: dd-MM-yyyy
* `userEmailAddress` - _optional_ - optional email address of user to return statistics for a single user, default is to return statistics for all users if administrator, or statistics for your own account if not an administrator
* `campaign` - _optional_ - optional campaign name
* `includeRefundedAndOptout` - _optional_ - optionally include refunded and optout counts, default is false
* `calculateCreditValue` - _optional_ - optionally calculate using credit value rather than message count, default is false

### transfer

> Transfers credits between two users in the same team. The <i>account email address</i> fields as well as the <i>number of credits to transfer</i> are required.

*Tags:* `account`

### search

> Find a user for a particular email address

*Tags:* `account`

#### Input Parameters
* `searchEmail` - _required_ - search by email address

### create

> Creates a new sub-account in your team. The following fields are required <i>firstname, lastname, email address, contact number</i> and <i>password.</i>

*Tags:* `account`

### getUser

> Gets a user from a given user id

*Tags:* `account`

#### Input Parameters
* `userId` - _required_ - userId

### update

> Updates a sub-account in your team. The following fields can be updated <i>firstname, lastname, contact number</i> and <i>password.</i>

*Tags:* `account`

#### Input Parameters
* `userId` - _required_ - userId

### all

> Returns all contacts

*Tags:* `contacts`

### create

> Creates a  contact

*Tags:* `contacts`

### delete

> Deletes a  contact

*Tags:* `contacts`

#### Input Parameters
* `contactId` - _required_ - contactId

### get

> Returns details for a single contact

*Tags:* `contacts`

#### Input Parameters
* `contactId` - _required_ - contactId

### update

> Updates a  contact

*Tags:* `contacts`

#### Input Parameters
* `contactId` - _required_ - contactId

### removeFromGroup

> Remove a contact from a group

*Tags:* `contacts`

#### Input Parameters
* `contactId` - _required_ - contactId
* `groupId` - _required_ - groupId

### removeFromGroup

> Remove a contact from a group

*Tags:* `contacts`

#### Input Parameters
* `contactId` - _required_ - contactId
* `groupId` - _required_ - groupId

### addToGroup

> Add a contact to a group

*Tags:* `contacts`

#### Input Parameters
* `contactId` - _required_ - contactId
* `groupId` - _required_ - groupId

### addToGroup

> Add a contact to a group

*Tags:* `contacts`

#### Input Parameters
* `contactId` - _required_ - contactId
* `groupId` - _required_ - groupId

### lookup

> Returns context information for a single provided

*Tags:* `context`

### lookup

> Returns context information for a single provided

*Tags:* `context`

### all

> Returns all groups

*Tags:* `groups`

### create

> Create a  group

*Tags:* `groups`

### delete

> Deletes a  group

*Tags:* `groups`

#### Input Parameters
* `groupId` - _required_ - groupId

### get

> Returns details for a single group

*Tags:* `groups`

#### Input Parameters
* `groupId` - _required_ - groupId

### update

> Update a  group

*Tags:* `groups`

#### Input Parameters
* `groupId` - _required_ - groupId

### addContact

> Add a contact to a group

*Tags:* `groups`

#### Input Parameters
* `groupId` - _required_ - groupId
* `contactId` - _required_ - contactId

### addContact

> Add a contact to a group

*Tags:* `groups`

#### Input Parameters
* `groupId` - _required_ - groupId
* `contactId` - _required_ - contactId

### removeContact

> Remove a contact from a group

*Tags:* `groups`

#### Input Parameters
* `groupId` - _required_ - groupId
* `contactId` - _required_ - contactId

### removeContact

> Remove a contact from a group

*Tags:* `groups`

#### Input Parameters
* `groupId` - _required_ - groupId
* `contactId` - _required_ - contactId

### all

> Returns all messages

*Tags:* `messages`

#### Input Parameters
* `pageSize` - _optional_ - number of elements to return at a time
* `page` - _optional_ - page number
* `type` - _optional_ - filter by message type
    Possible values: OUTBOUND, INBOUND.
* `status` - _optional_ - filter by message status
    Possible values: SCHEDULED, UNKNOWN, SENT, FAILED, FAILED_REFUNDED, FAILED_OPTOUT, DELIVERED.
* `fromDateTimeSent` - _optional_ - date format: yyyyMMdd
* `toDateTimeSent` - _optional_ - date format: yyyyMMdd
* `fromDateTimeReceived` - _optional_ - date format: yyyyMMdd
* `toDateTimeReceived` - _optional_ - date format: yyyyMMdd
* `fromNumber` - _optional_ - phone number the message was sent from
* `toNumber` - _optional_ - phone number the message was sent to
* `message` - _optional_ - search matching message text
* `campaign` - _optional_ - search by campaign
* `dataField` - _optional_ - search by data field
* `deleted` - _optional_ - return only deleted / not deleted messages
* `read` - _optional_ - return only read / unread messages (inbox messages only)
* `repliesToMessageId` - _optional_ - return only inbox messages which are a reply to the message with the given message id

### analyse-full

> Returns full analysis of message

*Tags:* `messages`

### analyse-message-credit-cost

> Returns the number of credit which would be required to send the request message to the requested recipient number

*Tags:* `messages`

### analyse-message-encoding

> Returns the message encoding that would be required to send the requested message

*Tags:* `messages`

### analyse-message-length

> Returns the number of characters the requested message consists of

*Tags:* `messages`

### analyse-

> Returns details for a single message

*Tags:* `messages`

### analyse-number-of-messages

> Returns the number of SMS parts which would be sent when sending the requested message

*Tags:* `messages`

### delete

> Deletes a  message

*Tags:* `messages`

#### Input Parameters
* `messageId` - _required_ - messageId

### get

> Returns details for a single message

*Tags:* `messages`

#### Input Parameters
* `messageId` - _required_ - messageId

### markRead

> Marks a  message as read

*Tags:* `messages`

#### Input Parameters
* `messageId` - _required_ - messageId

### markRead

> Marks a  message as read

*Tags:* `messages`

#### Input Parameters
* `messageId` - _required_ - messageId

### markUnread

> Marks a  message as unread

*Tags:* `messages`

#### Input Parameters
* `messageId` - _required_ - messageId

### markUnread

> Marks a  message as unread

*Tags:* `messages`

#### Input Parameters
* `messageId` - _required_ - messageId

### send

> Returns an example of the data to POST to send a single message.

*Tags:* `sms`

### send

> Sends a single message. The <i>recipientNumber</i> and <i>message</i> fields are required. All other fields are optional.

*Tags:* `sms`

### send-bulk

> Returns an example of the data to POST to send multiple messages in one transaction.

*Tags:* `sms`

### send-bulk

> Send multiple messages in one transaction.

*Tags:* `sms`

### send-url-parameters

> Send a single message using URL parameters.The <i>recipientNumber</i> and <i>message</i> parameters are required. All other parameters are optional.

*Tags:* `sms`

#### Input Parameters
* `recipientNumber` - _required_ - the phone number of the recipient to send to
* `message` - _required_ - the message to send
* `dateToSend` - _optional_ - date format: yyyyMMddHHmm
* `campaign` - _optional_ - optional campaign name
* `dataField` - _optional_ - optional extra data

### send-url-parameters

> Send a single message using URL parameters.The <i>recipientNumber</i> and <i>message</i> parameters are required. All other parameters are optional.

*Tags:* `sms`

#### Input Parameters
* `recipientNumber` - _required_ - the phone number of the recipient to send to
* `message` - _required_ - the message to send
* `dateToSend` - _optional_ - date format: yyyyMMddHHmm
* `campaign` - _optional_ - optional campaign name
* `dataField` - _optional_ - optional extra data

### send-url

> Send a single message using your unique URL without having to authenticate using your email address or REST API token. The token required is the URL Sending token available on the developer setting page. The <i>recipientNumber</i> and <i>message</i> parameters are required. All other parameters are optional. Not that the token required here is

*Tags:* `sms`

#### Input Parameters
* `token` - _required_ - token
* `recipientNumber` - _required_ - the phone number of the recipient to send to
* `message` - _required_ - the message to send
* `dateToSend` - _optional_ - date format: yyyyMMddHHmm
* `campaign` - _optional_ - optional campaign name
* `dataField` - _optional_ - optional extra data

### send-url

> Send a single message using your unique URL without having to authenticate using your email address or REST API token. The token required is the URL Sending token available on the developer setting page. The <i>recipientNumber</i> and <i>message</i> parameters are required. All other parameters are optional. Not that the token required here is

*Tags:* `sms`

#### Input Parameters
* `token` - _required_ - token
* `recipientNumber` - _required_ - the phone number of the recipient to send to
* `message` - _required_ - the message to send
* `dateToSend` - _optional_ - date format: yyyyMMddHHmm
* `campaign` - _optional_ - optional campaign name
* `dataField` - _optional_ - optional extra data

### all

> Returns all templates

*Tags:* `templates`

### delete

> Deletes a  template

*Tags:* `templates`

#### Input Parameters
* `templateId` - _required_ - templateId

### get

> Returns details for a single template

*Tags:* `templates`

#### Input Parameters
* `templateId` - _required_ - templateId

### all

> Returns all voice messages

*Tags:* `voice`

#### Input Parameters
* `pageSize` - _optional_ - number of elements to return at a time
* `page` - _optional_ - page number
* `status` - _optional_ - filter by message status
    Possible values: SCHEDULED, UNKNOWN, SENT, FAILED, FAILED_REFUNDED, FAILED_OPTOUT, DELIVERED.
* `fromDateTimeSent` - _optional_ - date format: yyyyMMdd
* `toDateTimeSent` - _optional_ - date format: yyyyMMdd
* `toNumber` - _optional_ - phone number the message was sent to
* `message` - _optional_ - search matching message text
* `campaign` - _optional_ - search by campaign
* `dataField` - _optional_ - search by data field
* `deleted` - _optional_ - return only deleted / not deleted messages

### single-audio

> Send a single audio voice message to one recipient. Note, Content-Type header must be set to multipart/form-data for this request.

*Tags:* `voice`

#### Input Parameters
* `recipientNumber` - _required_ - the phone number of the recipient to send to
* `campaign` - _optional_ - optional campaign name
* `dataField` - _optional_ - optional extra data
* `retryCount` - _optional_ - optional number of times to retry unanswered call
* `retryMinimumInterval` - _optional_ - optional minimum interval in minutes between retry attempts
* `retryMaximumInterval` - _optional_ - optional maximum interval in minutes between retry attempts

### single-text

> Send a single text voice message to one recipient

*Tags:* `voice`

### delete

> Deletes a  message

*Tags:* `voice`

#### Input Parameters
* `messageId` - _required_ - messageId

### get

> Returns details for a single message

*Tags:* `voice`

#### Input Parameters
* `messageId` - _required_ - messageId

## License

**flow**ground :- Telekom iPaaS / zoomconnect-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
