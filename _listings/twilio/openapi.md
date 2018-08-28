swagger: "2.0"
x-collection-name: Twilio
x-complete: 1
info:
  title: Twilio
  description: twilio-is-a-cloud-communications-infrastructure-as-a-serviceiaas-company-based-in-san-francisco-california--twilio-allows-software-developers-to-programmatically-make-and-receive-phone-calls-and-send-and-receive-text-messages-using-its-web-service-apis--twilios-services-are-accessed-over-http-and-are-billed-based-on-usage-
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/Messages.{format}:
    get:
      summary: Get Message Media
      description: Returns a list of messages associated with your account. The list
        includes paging information.
      operationId: returns-a-list-of-messages-associated-with-your-account-the-list-includes-paging-information
      x-api-path-slug: accountsaccountsidmessages-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Messages
  /Accounts/{AccountSid}/Messages/{MessageSid}:
    get:
      summary: Get Message Media
      description: Returns a single message specified by the provided {MessageSid}.n
      operationId: returns-a-single-message-specified-by-the-provided-messagesid
      x-api-path-slug: accountsaccountsidmessagesmessagesid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: MessageSid
        description: A 34 character string that uniquely identifies the message
      responses:
        200:
          description: OK
      tags:
      - Messages
  /Accounts/{AccountSid}/Messages/{MessageSid}/Media:
    get:
      summary: Get Message Media
      description: Returns a list of media associated with your message.
      operationId: returns-a-list-of-media-associated-with-your-message
      x-api-path-slug: accountsaccountsidmessagesmessagesidmedia-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: MessageSid
        description: A 34 character string that uniquely identifies the message
      responses:
        200:
          description: OK
      tags:
      - Messages
  /Accounts/{AccountSid}/Messages/{MessageSid}/Media/{MediaSid}:
    get:
      summary: Get Message Media
      description: Without an extension, the media is returned using the mime-type
        provided when the media was generated.
      operationId: without-an-extension-the-media-is-returned-using-the-mimetype-provided-when-the-media-was-generated
      x-api-path-slug: accountsaccountsidmessagesmessagesidmediamediasid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: MediaSid
        description: A 34 character string that uniquely identifies the media object
      - in: path
        name: MessageSid
        description: A 34 character string that uniquely identifies the message
      responses:
        200:
          description: OK
      tags:
      - Messages
  /Accounts/{AccountSid}/SMS/ShortCodes:
    get:
      summary: Get SMS Short Code Media
      description: Returns a list of ShortCode resource representations, each representing
        anshort code within your account. The list includes paging information.n
      operationId: returns-a-list-of-shortcode-resource-representations-each-representing-ashort-code-within-your-accou
      x-api-path-slug: accountsaccountsidsmsshortcodes-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Short Codes
  /Accounts/{AccountSid}/SMS/ShortCodes/{ShortCodeSid}:
    get:
      summary: Get SMS Short Code Media
      description: Get a single message.
      operationId: get-a-single-message
      x-api-path-slug: accountsaccountsidsmsshortcodesshortcodesid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: ShortCodeSid
      responses:
        200:
          description: OK
      tags:
      - Short Codes
    post:
      summary: Add SMS Short Code Media
      description: Tries to update the shortcodes properties, and returns the updatednresource
        representation if successful.n
      operationId: tries-to-update-the-shortcodes-properties-and-returns-the-updatedresource-representation-if-successf
      x-api-path-slug: accountsaccountsidsmsshortcodesshortcodesid-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: ShortCodeSid
      responses:
        200:
          description: OK
      tags:
      - Short Codes