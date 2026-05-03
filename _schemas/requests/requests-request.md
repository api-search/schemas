---
description: JSON Schema describing the parameters accepted by the Python Requests library's main request() function and convenience methods (get, post, put, patch, delete, head, options).
layout: schema
name: Requests Request
properties_list:
- description: HTTP method for the request.
  name: method
  type: string
- description: URL for the request.
  name: url
  type: string
- description: Dictionary, list of tuples, or bytes to send in the query string.
  name: params
  type:
  - object
  - array
  - string
- description: Dictionary, list of tuples, bytes, or file-like object to send in the request body (form-encoded).
  name: data
  type:
  - object
  - array
  - string
- description: A JSON-serializable Python object to send as application/json in the request body.
  name: json
  type: object
- description: Dictionary of HTTP headers to send with the request.
  name: headers
  type: object
- description: Dictionary or CookieJar of cookies to send with the request.
  name: cookies
  type:
  - object
  - string
- description: Dictionary of name to file-like objects for multipart form upload.
  name: files
  type: object
- description: Auth tuple (username, password) for Basic Auth, or an auth callable for custom auth schemes.
  name: auth
  type:
  - array
  - object
  - 'null'
- description: Seconds to wait for the server to respond. Float for single timeout; [connect_timeout, read_timeout] tuple for separate timeouts.
  name: timeout
  type:
  - number
  - array
  - 'null'
- description: Whether to follow redirects. Defaults to True for GET/POST/etc., False for HEAD.
  name: allow_redirects
  type: boolean
- description: 'Dictionary mapping protocol schemes to proxy URLs (e.g., {''https'': ''http://proxy:8080''}).'
  name: proxies
  type: object
- description: Boolean to control TLS certificate verification, or path string to a CA bundle. Defaults to True.
  name: verify
  type:
  - boolean
  - string
- description: If False, response content is downloaded immediately. If True, streaming mode is used.
  name: stream
  type: boolean
- description: Path to SSL client certificate .pem file, or a ['cert', 'key'] tuple.
  name: cert
  type:
  - string
  - array
provider_name: Requests
provider_slug: requests
schema_file: json-schema/requests-request-schema.json
slug: requests-request
source_filename: requests-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/requests/refs/heads/main/json-schema/requests-request-schema.json\",\n  \"title\": \"Requests Request\",\n  \"description\": \"JSON Schema describing the parameters accepted by the Python Requests library's main request() function and convenience methods (get, post, put, patch, delete, head, options).\",\n  \"type\": \"object\",\n  \"required\": [\"method\", \"url\"],\n  \"properties\": {\n    \"method\": {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\", \"HEAD\", \"OPTIONS\"],\n      \"description\": \"HTTP method for the request.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the request.\"\n    },\n    \"params\": {\n      \"type\": [\"object\", \"array\", \"string\"],\n      \"description\": \"Dictionary, list of tuples, or\
  \ bytes to send in the query string.\"\n    },\n    \"data\": {\n      \"type\": [\"object\", \"array\", \"string\"],\n      \"description\": \"Dictionary, list of tuples, bytes, or file-like object to send in the request body (form-encoded).\"\n    },\n    \"json\": {\n      \"description\": \"A JSON-serializable Python object to send as application/json in the request body.\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Dictionary of HTTP headers to send with the request.\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"cookies\": {\n      \"type\": [\"object\", \"string\"],\n      \"description\": \"Dictionary or CookieJar of cookies to send with the request.\"\n    },\n    \"files\": {\n      \"type\": \"object\",\n      \"description\": \"Dictionary of name to file-like objects for multipart form upload.\"\n    },\n    \"auth\": {\n      \"type\": [\"array\", \"object\", \"null\"],\n      \"description\": \"Auth tuple\
  \ (username, password) for Basic Auth, or an auth callable for custom auth schemes.\"\n    },\n    \"timeout\": {\n      \"type\": [\"number\", \"array\", \"null\"],\n      \"description\": \"Seconds to wait for the server to respond. Float for single timeout; [connect_timeout, read_timeout] tuple for separate timeouts.\"\n    },\n    \"allow_redirects\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to follow redirects. Defaults to True for GET/POST/etc., False for HEAD.\",\n      \"default\": true\n    },\n    \"proxies\": {\n      \"type\": \"object\",\n      \"description\": \"Dictionary mapping protocol schemes to proxy URLs (e.g., {'https': 'http://proxy:8080'}).\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"verify\": {\n      \"type\": [\"boolean\", \"string\"],\n      \"description\": \"Boolean to control TLS certificate verification, or path string to a CA bundle. Defaults to True.\",\n      \"default\": true\n    },\n    \"stream\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"If False, response content is downloaded immediately. If True, streaming mode is used.\",\n      \"default\": false\n    },\n    \"cert\": {\n      \"type\": [\"string\", \"array\"],\n      \"description\": \"Path to SSL client certificate .pem file, or a ['cert', 'key'] tuple.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/requests/refs/heads/main/json-schema/requests-request-schema.json
tags:
- Clients
- HTTP Client
- HTTP Library
- Open Source
- Python
- Python Software Foundation
title: Requests Request
---
