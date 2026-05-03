---
description: JSON Schema representing the key attributes of a requests.Response object returned by the Python Requests library after an HTTP call.
layout: schema
name: Requests Response
properties_list:
- description: HTTP status code of the response (e.g., 200, 404, 500).
  name: status_code
  type: integer
- description: True if status_code is less than 400, False otherwise.
  name: ok
  type: boolean
- description: Final URL of the response after following any redirects.
  name: url
  type: string
- description: Case-insensitive dictionary of response headers.
  name: headers
  type: object
- description: Encoding to use when accessing response.text. Guessed from Content-Type header.
  name: encoding
  type:
  - string
  - 'null'
- description: Response body decoded as a string using response.encoding.
  name: text
  type: string
- description: Response body as raw bytes (base64-encoded for JSON representation).
  name: content
  type: string
- description: Parsed JSON body, equivalent to calling response.json(). Only present when Content-Type is application/json.
  name: json_body
  type:
  - object
  - array
  - 'null'
- description: Time elapsed between sending the request and receiving the last byte of the response, in seconds.
  name: elapsed
  type: number
- description: List of Response objects representing any redirects followed.
  name: history
  type: array
- description: CookieJar of cookies the server sent back.
  name: cookies
  type: object
- description: HTTP reason phrase for the status code (e.g., 'OK', 'Not Found').
  name: reason
  type: string
- description: The PreparedRequest object that was sent.
  name: request
  type: object
provider_name: Requests
provider_slug: requests
schema_file: json-schema/requests-response-schema.json
slug: requests-response
source_filename: requests-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/requests/refs/heads/main/json-schema/requests-response-schema.json\",\n  \"title\": \"Requests Response\",\n  \"description\": \"JSON Schema representing the key attributes of a requests.Response object returned by the Python Requests library after an HTTP call.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status_code\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code of the response (e.g., 200, 404, 500).\",\n      \"examples\": [200, 201, 400, 404, 500]\n    },\n    \"ok\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if status_code is less than 400, False otherwise.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Final URL of the response after following any redirects.\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Case-insensitive dictionary of response headers.\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"encoding\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Encoding to use when accessing response.text. Guessed from Content-Type header.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Response body decoded as a string using response.encoding.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"contentEncoding\": \"base64\",\n      \"description\": \"Response body as raw bytes (base64-encoded for JSON representation).\"\n    },\n    \"json_body\": {\n      \"type\": [\"object\", \"array\", \"null\"],\n      \"description\": \"Parsed JSON body, equivalent to calling response.json(). Only present when Content-Type is application/json.\"\n    },\n    \"elapsed\": {\n      \"type\": \"number\",\n      \"description\": \"Time elapsed between sending the request and receiving\
  \ the last byte of the response, in seconds.\"\n    },\n    \"history\": {\n      \"type\": \"array\",\n      \"description\": \"List of Response objects representing any redirects followed.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A redirect response in the redirect chain.\"\n      }\n    },\n    \"cookies\": {\n      \"type\": \"object\",\n      \"description\": \"CookieJar of cookies the server sent back.\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP reason phrase for the status code (e.g., 'OK', 'Not Found').\"\n    },\n    \"request\": {\n      \"type\": \"object\",\n      \"description\": \"The PreparedRequest object that was sent.\",\n      \"properties\": {\n        \"method\": { \"type\": \"string\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"headers\": { \"type\": \"object\" },\n        \"body\": { \"\
  type\": [\"string\", \"null\"] }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/requests/refs/heads/main/json-schema/requests-response-schema.json
tags:
- Clients
- HTTP Client
- HTTP Library
- Open Source
- Python
- Python Software Foundation
title: Requests Response
---
