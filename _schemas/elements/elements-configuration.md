---
description: Configuration properties for the Stoplight Elements API React component and elements-api Web Component. These options control the OpenAPI specification source, display layout, navigation routing, Try It console behavior, and visibility of individual UI sections.
layout: schema
name: Stoplight Elements Configuration
properties_list:
- description: URL pointing to the OpenAPI 2.0, 3.0, or 3.1 specification document to render. Mutually exclusive with apiDescriptionDocument.
  name: apiDescriptionUrl
  type: string
- description: The OpenAPI 2.0, 3.0, or 3.1 document provided directly as a JSON string, YAML string, or parsed JavaScript object. Mutually exclusive with apiDescriptionUrl.
  name: apiDescriptionDocument
  type: object
- description: Controls the visual layout of the rendered documentation. sidebar places navigation on the left side resembling Stoplight Platform. stacked renders a single-column layout resembling Swagger UI with no
  name: layout
  type: string
- description: Controls the routing strategy used for deep-linking to individual operations and schemas. hash uses URL hash fragments. history uses the HTML5 History API. memory keeps navigation state in memory with
  name: router
  type: string
- description: The base path prefix for the router when using history or hash routing. Useful when Elements is embedded at a non-root URL path.
  name: basePath
  type: string
- description: A static path override used with the static router option to render a specific operation or schema without URL-based navigation.
  name: staticRouterPath
  type: string
- description: URL of an image to display as the logo in the sidebar above the navigation. Only applies when layout is sidebar or responsive.
  name: logo
  type: string
- description: When true, hides the Try It console tab from all operation pages. Users cannot send test requests from the documentation.
  name: hideTryIt
  type: boolean
- description: When true, hides the right panel containing the Try It console and request samples, showing only the operation documentation without the request/response panel.
  name: hideTryItPanel
  type: boolean
- description: When true, hides the automatically generated request code samples panel from operation documentation pages.
  name: hideSamples
  type: boolean
- description: When true, hides all schema definitions from the sidebar Table of Contents navigation. Schema objects from the components/schemas section are not linked in the sidebar.
  name: hideSchemas
  type: boolean
- description: When true, hides all operations and models marked as internal using the x-internal vendor extension. Internal operations are not displayed in the documentation or sidebar navigation.
  name: hideInternal
  type: boolean
- description: When true, hides the Export button from the API overview page. Users cannot download the OpenAPI specification from the rendered documentation page.
  name: hideExport
  type: boolean
- description: When true, hides the Server information section from the API overview and operation pages.
  name: hideServerInfo
  type: boolean
- description: When true, hides the Security information section from the API overview and operation pages.
  name: hideSecurityInfo
  type: boolean
- description: Controls the credentials fetch policy for requests sent from the Try It console. omit sends no cookies or authorization headers. include always sends credentials. same-origin sends credentials only fo
  name: tryItCredentialsPolicy
  type: string
- description: URL of a CORS proxy server that will be prepended to the request URL when sending Try It requests. Use this when the target API does not allow cross-origin requests from the browser.
  name: tryItCorsProxy
  type: string
- description: Maximum depth for resolving and rendering inline $ref references in schemas. Prevents infinite loops in deeply recursive or circular schemas. When not set, defaults to the Elements internal maximum.
  name: maxRefDepth
  type: integer
- description: When true, indicates that Elements is nested inside an existing router (such as React Router) in the parent application. Elements will use the outer router context rather than creating its own interna
  name: outerRouter
  type: boolean
- description: A reference to a custom renderer function for vendor extensions (x- fields) in the OpenAPI document. Allows applications to provide custom UI renderers for specification extensions. Only applicable in
  name: renderExtensionAddon
  type: string
provider_name: Stoplight Elements
provider_slug: elements
schema_file: json-schema/elements-configuration-schema.json
slug: elements-configuration
source_filename: elements-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://apievangelist.com/schemas/elements/elements-configuration.json\",\n  \"title\": \"Stoplight Elements Configuration\",\n  \"description\": \"Configuration properties for the Stoplight Elements API React component and elements-api Web Component. These options control the OpenAPI specification source, display layout, navigation routing, Try It console behavior, and visibility of individual UI sections.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiDescriptionUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL pointing to the OpenAPI 2.0, 3.0, or 3.1 specification document to render. Mutually exclusive with apiDescriptionDocument.\",\n      \"examples\": [\"https://api.example.com/openapi.json\"]\n    },\n    \"apiDescriptionDocument\": {\n      \"oneOf\": [\n        {\n          \"type\": \"string\",\n          \"description\": \"The\
  \ OpenAPI document as a JSON or YAML string.\"\n        },\n        {\n          \"type\": \"object\",\n          \"description\": \"The OpenAPI document as a pre-parsed JavaScript object.\"\n        }\n      ],\n      \"description\": \"The OpenAPI 2.0, 3.0, or 3.1 document provided directly as a JSON string, YAML string, or parsed JavaScript object. Mutually exclusive with apiDescriptionUrl.\"\n    },\n    \"layout\": {\n      \"type\": \"string\",\n      \"enum\": [\"sidebar\", \"stacked\", \"responsive\"],\n      \"default\": \"sidebar\",\n      \"description\": \"Controls the visual layout of the rendered documentation. sidebar places navigation on the left side resembling Stoplight Platform. stacked renders a single-column layout resembling Swagger UI with no sidebar. responsive automatically switches between sidebar and stacked based on viewport width.\"\n    },\n    \"router\": {\n      \"type\": \"string\",\n      \"enum\": [\"hash\", \"memory\", \"history\", \"static\"],\n  \
  \    \"description\": \"Controls the routing strategy used for deep-linking to individual operations and schemas. hash uses URL hash fragments. history uses the HTML5 History API. memory keeps navigation state in memory without modifying the URL. static disables routing entirely.\"\n    },\n    \"basePath\": {\n      \"type\": \"string\",\n      \"description\": \"The base path prefix for the router when using history or hash routing. Useful when Elements is embedded at a non-root URL path.\",\n      \"examples\": [\"/api-docs\"]\n    },\n    \"staticRouterPath\": {\n      \"type\": \"string\",\n      \"description\": \"A static path override used with the static router option to render a specific operation or schema without URL-based navigation.\"\n    },\n    \"logo\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of an image to display as the logo in the sidebar above the navigation. Only applies when layout is sidebar or responsive.\",\n \
  \     \"examples\": [\"https://example.com/logo.png\"]\n    },\n    \"hideTryIt\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"When true, hides the Try It console tab from all operation pages. Users cannot send test requests from the documentation.\"\n    },\n    \"hideTryItPanel\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"When true, hides the right panel containing the Try It console and request samples, showing only the operation documentation without the request/response panel.\"\n    },\n    \"hideSamples\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"When true, hides the automatically generated request code samples panel from operation documentation pages.\"\n    },\n    \"hideSchemas\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"When true, hides all schema definitions from the sidebar Table of Contents navigation.\
  \ Schema objects from the components/schemas section are not linked in the sidebar.\"\n    },\n    \"hideInternal\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"When true, hides all operations and models marked as internal using the x-internal vendor extension. Internal operations are not displayed in the documentation or sidebar navigation.\"\n    },\n    \"hideExport\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"When true, hides the Export button from the API overview page. Users cannot download the OpenAPI specification from the rendered documentation page.\"\n    },\n    \"hideServerInfo\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"When true, hides the Server information section from the API overview and operation pages.\"\n    },\n    \"hideSecurityInfo\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"When true, hides\
  \ the Security information section from the API overview and operation pages.\"\n    },\n    \"tryItCredentialsPolicy\": {\n      \"type\": \"string\",\n      \"enum\": [\"omit\", \"include\", \"same-origin\"],\n      \"default\": \"omit\",\n      \"description\": \"Controls the credentials fetch policy for requests sent from the Try It console. omit sends no cookies or authorization headers. include always sends credentials. same-origin sends credentials only for same-origin requests. Maps to the credentials option of the Fetch API.\"\n    },\n    \"tryItCorsProxy\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of a CORS proxy server that will be prepended to the request URL when sending Try It requests. Use this when the target API does not allow cross-origin requests from the browser.\",\n      \"examples\": [\"https://cors-anywhere.example.com/\"]\n    },\n    \"maxRefDepth\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n     \
  \ \"description\": \"Maximum depth for resolving and rendering inline $ref references in schemas. Prevents infinite loops in deeply recursive or circular schemas. When not set, defaults to the Elements internal maximum.\",\n      \"examples\": [5]\n    },\n    \"outerRouter\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"When true, indicates that Elements is nested inside an existing router (such as React Router) in the parent application. Elements will use the outer router context rather than creating its own internal router instance.\"\n    },\n    \"renderExtensionAddon\": {\n      \"type\": \"string\",\n      \"description\": \"A reference to a custom renderer function for vendor extensions (x- fields) in the OpenAPI document. Allows applications to provide custom UI renderers for specification extensions. Only applicable in React usage.\"\n    }\n  },\n  \"additionalProperties\": false,\n  \"$defs\": {\n    \"LayoutOption\": {\n      \"type\"\
  : \"string\",\n      \"enum\": [\"sidebar\", \"stacked\", \"responsive\"],\n      \"description\": \"Available display layout modes for the Elements component. sidebar renders a three-panel layout with navigation sidebar. stacked renders all content in a single scrollable column. responsive switches between sidebar and stacked based on viewport width.\"\n    },\n    \"RouterOption\": {\n      \"type\": \"string\",\n      \"enum\": [\"hash\", \"memory\", \"history\", \"static\"],\n      \"description\": \"Available routing strategies for deep-linking within the Elements component. hash uses URL hash fragments. history uses the HTML5 History API push state. memory keeps state in memory without modifying the browser URL. static disables client-side routing entirely.\"\n    },\n    \"CredentialsPolicy\": {\n      \"type\": \"string\",\n      \"enum\": [\"omit\", \"include\", \"same-origin\"],\n      \"description\": \"Fetch API credentials policy for the Try It console. Controls whether cookies\
  \ and HTTP authentication credentials are sent with outgoing requests.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/elements/refs/heads/main/json-schema/elements-configuration-schema.json
tags:
- API Documentation
- Developer Tools
- Documentation
- Interactive Docs
- OpenAPI
- React
- Web Components
title: Stoplight Elements Configuration
---
