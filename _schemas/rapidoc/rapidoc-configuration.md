---
description: Configuration attributes for the rapi-doc custom HTML element that renders OpenAPI specifications as interactive API documentation.
layout: schema
name: RapiDoc Web Component Configuration
properties_list:
- description: URL of the OpenAPI specification to render.
  name: spec-url
  type: string
- description: When true, updates the browser URL hash as the user navigates through the API documentation.
  name: update-route
  type: boolean
- description: Prefix to add to route paths in the URL hash.
  name: route-prefix
  type: string
- description: Sort tags alphabetically.
  name: sort-tags
  type: boolean
- description: Sort order for endpoints within each tag.
  name: sort-endpoints-by
  type: string
- description: Custom heading text to display in the header.
  name: heading-text
  type: string
- description: Initial path to navigate to when the component loads.
  name: goto-path
  type: string
- description: Pre-fill request fields with example values from the spec.
  name: fill-request-fields-with-example
  type: boolean
- description: Persist authentication data in localStorage across sessions.
  name: persist-auth
  type: boolean
- description: Color theme for the documentation UI.
  name: theme
  type: string
- description: Background color for the documentation page.
  name: bg-color
  type: string
- description: Primary text color.
  name: text-color
  type: string
- description: Background color for the header bar.
  name: header-color
  type: string
- description: Primary accent color used for links, buttons, and highlights.
  name: primary-color
  type: string
- description: Background color for the navigation sidebar.
  name: nav-bg-color
  type: string
- description: Text color for the navigation sidebar.
  name: nav-text-color
  type: string
- description: Hover background color for navigation items.
  name: nav-hover-bg-color
  type: string
- description: Hover text color for navigation items.
  name: nav-hover-text-color
  type: string
- description: Accent color for active and highlighted navigation items.
  name: nav-accent-color
  type: string
- description: Text color on accented navigation items.
  name: nav-accent-text-color
  type: string
- description: Spacing between navigation items.
  name: nav-item-spacing
  type: string
- description: Show endpoint paths instead of summaries in the navigation bar.
  name: use-path-in-nav-bar
  type: boolean
- description: Show headings from the info description as navigation items.
  name: info-description-headings-in-navbar
  type: boolean
- description: Base font size for the documentation.
  name: font-size
  type: string
- description: Font family for regular body text.
  name: regular-font
  type: string
- description: Font family for monospaced/code text.
  name: mono-font
  type: string
- description: Whether to load default Google fonts.
  name: load-fonts
  type: boolean
- description: Layout rendering style. 'read' shows request/response side by side, 'view' shows them stacked, 'focused' shows one endpoint at a time.
  name: render-style
  type: string
- description: Layout direction. 'row' places nav on the side, 'column' stacks everything vertically.
  name: layout
  type: string
- description: Height of the response area in the Try It console.
  name: response-area-height
  type: string
- description: Show the API info section at the top.
  name: show-info
  type: boolean
- description: Show the schema components section.
  name: show-components
  type: boolean
- description: Show the header bar.
  name: show-header
  type: boolean
- description: Allow users to configure authentication.
  name: allow-authentication
  type: boolean
- description: Show the Try It console for making live API requests.
  name: allow-try
  type: boolean
- description: Allow users to load a different spec URL from the UI.
  name: allow-spec-url-load
  type: boolean
- description: Allow users to load a spec file from the local filesystem.
  name: allow-spec-file-load
  type: boolean
- description: Show option to download the spec file.
  name: allow-spec-file-download
  type: boolean
- description: Show the search bar in the header.
  name: allow-search
  type: boolean
- description: Show advanced search options.
  name: allow-advanced-search
  type: boolean
- description: Allow users to select a server from the servers list.
  name: allow-server-selection
  type: boolean
- description: Allow toggling expansion of schema descriptions.
  name: allow-schema-description-expand-toggle
  type: boolean
- description: Display style for schema definitions.
  name: schema-style
  type: string
- description: Number of schema levels to expand by default.
  name: schema-expand-level
  type: integer
- description: Expand schema descriptions by default.
  name: schema-description-expanded
  type: boolean
- description: When to hide read-only schema properties.
  name: schema-hide-read-only
  type: string
- description: When to hide write-only schema properties.
  name: schema-hide-write-only
  type: string
- description: Default tab to show for schema sections.
  name: default-schema-tab
  type: string
- description: Name of the API key header or query parameter for authentication.
  name: api-key-name
  type: string
- description: Location of the API key (header or query parameter).
  name: api-key-location
  type: string
- description: Default value for the API key.
  name: api-key-value
  type: string
- description: Default server URL to use for API requests.
  name: server-url
  type: string
- description: URL of the default API server from the servers list.
  name: default-api-server
  type: string
- description: Credentials policy for fetch requests made from the Try It console.
  name: fetch-credentials
  type: string
- description: Search match type for filtering endpoints.
  name: match-type
  type: string
provider_name: RapiDoc
provider_slug: rapidoc
schema_file: json-schema/rapidoc-configuration.json
slug: rapidoc-configuration
source_filename: rapidoc-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/rapidoc/blob/main/json-schema/rapidoc-configuration.json\",\n  \"title\": \"RapiDoc Web Component Configuration\",\n  \"description\": \"Configuration attributes for the rapi-doc custom HTML element that renders OpenAPI specifications as interactive API documentation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spec-url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the OpenAPI specification to render.\"\n    },\n    \"update-route\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"When true, updates the browser URL hash as the user navigates through the API documentation.\"\n    },\n    \"route-prefix\": {\n      \"type\": \"string\",\n      \"description\": \"Prefix to add to route paths in the URL hash.\"\n    },\n    \"sort-tags\": {\n      \"type\": \"boolean\"\
  ,\n      \"default\": false,\n      \"description\": \"Sort tags alphabetically.\"\n    },\n    \"sort-endpoints-by\": {\n      \"type\": \"string\",\n      \"enum\": [\"path\", \"method\", \"summary\", \"none\"],\n      \"default\": \"path\",\n      \"description\": \"Sort order for endpoints within each tag.\"\n    },\n    \"heading-text\": {\n      \"type\": \"string\",\n      \"description\": \"Custom heading text to display in the header.\"\n    },\n    \"goto-path\": {\n      \"type\": \"string\",\n      \"description\": \"Initial path to navigate to when the component loads.\"\n    },\n    \"fill-request-fields-with-example\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Pre-fill request fields with example values from the spec.\"\n    },\n    \"persist-auth\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Persist authentication data in localStorage across sessions.\"\n    },\n    \"theme\": {\n      \"\
  type\": \"string\",\n      \"enum\": [\"light\", \"dark\"],\n      \"default\": \"light\",\n      \"description\": \"Color theme for the documentation UI.\"\n    },\n    \"bg-color\": {\n      \"type\": \"string\",\n      \"description\": \"Background color for the documentation page.\"\n    },\n    \"text-color\": {\n      \"type\": \"string\",\n      \"description\": \"Primary text color.\"\n    },\n    \"header-color\": {\n      \"type\": \"string\",\n      \"description\": \"Background color for the header bar.\"\n    },\n    \"primary-color\": {\n      \"type\": \"string\",\n      \"description\": \"Primary accent color used for links, buttons, and highlights.\"\n    },\n    \"nav-bg-color\": {\n      \"type\": \"string\",\n      \"description\": \"Background color for the navigation sidebar.\"\n    },\n    \"nav-text-color\": {\n      \"type\": \"string\",\n      \"description\": \"Text color for the navigation sidebar.\"\n    },\n    \"nav-hover-bg-color\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Hover background color for navigation items.\"\n    },\n    \"nav-hover-text-color\": {\n      \"type\": \"string\",\n      \"description\": \"Hover text color for navigation items.\"\n    },\n    \"nav-accent-color\": {\n      \"type\": \"string\",\n      \"description\": \"Accent color for active and highlighted navigation items.\"\n    },\n    \"nav-accent-text-color\": {\n      \"type\": \"string\",\n      \"description\": \"Text color on accented navigation items.\"\n    },\n    \"nav-item-spacing\": {\n      \"type\": \"string\",\n      \"enum\": [\"default\", \"compact\", \"relaxed\"],\n      \"default\": \"default\",\n      \"description\": \"Spacing between navigation items.\"\n    },\n    \"use-path-in-nav-bar\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Show endpoint paths instead of summaries in the navigation bar.\"\n    },\n    \"info-description-headings-in-navbar\": {\n      \"type\": \"boolean\"\
  ,\n      \"default\": false,\n      \"description\": \"Show headings from the info description as navigation items.\"\n    },\n    \"font-size\": {\n      \"type\": \"string\",\n      \"enum\": [\"default\", \"large\", \"largest\"],\n      \"default\": \"default\",\n      \"description\": \"Base font size for the documentation.\"\n    },\n    \"regular-font\": {\n      \"type\": \"string\",\n      \"description\": \"Font family for regular body text.\"\n    },\n    \"mono-font\": {\n      \"type\": \"string\",\n      \"description\": \"Font family for monospaced/code text.\"\n    },\n    \"load-fonts\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether to load default Google fonts.\"\n    },\n    \"render-style\": {\n      \"type\": \"string\",\n      \"enum\": [\"read\", \"view\", \"focused\"],\n      \"default\": \"read\",\n      \"description\": \"Layout rendering style. 'read' shows request/response side by side, 'view' shows them stacked,\
  \ 'focused' shows one endpoint at a time.\"\n    },\n    \"layout\": {\n      \"type\": \"string\",\n      \"enum\": [\"row\", \"column\"],\n      \"default\": \"row\",\n      \"description\": \"Layout direction. 'row' places nav on the side, 'column' stacks everything vertically.\"\n    },\n    \"response-area-height\": {\n      \"type\": \"string\",\n      \"default\": \"300px\",\n      \"description\": \"Height of the response area in the Try It console.\"\n    },\n    \"show-info\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Show the API info section at the top.\"\n    },\n    \"show-components\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Show the schema components section.\"\n    },\n    \"show-header\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Show the header bar.\"\n    },\n    \"allow-authentication\": {\n      \"type\": \"boolean\",\n      \"default\"\
  : true,\n      \"description\": \"Allow users to configure authentication.\"\n    },\n    \"allow-try\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Show the Try It console for making live API requests.\"\n    },\n    \"allow-spec-url-load\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Allow users to load a different spec URL from the UI.\"\n    },\n    \"allow-spec-file-load\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Allow users to load a spec file from the local filesystem.\"\n    },\n    \"allow-spec-file-download\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Show option to download the spec file.\"\n    },\n    \"allow-search\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Show the search bar in the header.\"\n    },\n    \"allow-advanced-search\": {\n      \"type\": \"boolean\",\n\
  \      \"default\": true,\n      \"description\": \"Show advanced search options.\"\n    },\n    \"allow-server-selection\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Allow users to select a server from the servers list.\"\n    },\n    \"allow-schema-description-expand-toggle\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Allow toggling expansion of schema descriptions.\"\n    },\n    \"schema-style\": {\n      \"type\": \"string\",\n      \"enum\": [\"tree\", \"table\"],\n      \"default\": \"tree\",\n      \"description\": \"Display style for schema definitions.\"\n    },\n    \"schema-expand-level\": {\n      \"type\": \"integer\",\n      \"default\": 999,\n      \"description\": \"Number of schema levels to expand by default.\"\n    },\n    \"schema-description-expanded\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Expand schema descriptions by default.\"\n  \
  \  },\n    \"schema-hide-read-only\": {\n      \"type\": \"string\",\n      \"enum\": [\"always\", \"never\", \"post,put,patch\"],\n      \"default\": \"always\",\n      \"description\": \"When to hide read-only schema properties.\"\n    },\n    \"schema-hide-write-only\": {\n      \"type\": \"string\",\n      \"enum\": [\"always\", \"never\"],\n      \"default\": \"always\",\n      \"description\": \"When to hide write-only schema properties.\"\n    },\n    \"default-schema-tab\": {\n      \"type\": \"string\",\n      \"enum\": [\"model\", \"example\"],\n      \"default\": \"model\",\n      \"description\": \"Default tab to show for schema sections.\"\n    },\n    \"api-key-name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the API key header or query parameter for authentication.\"\n    },\n    \"api-key-location\": {\n      \"type\": \"string\",\n      \"enum\": [\"header\", \"query\"],\n      \"description\": \"Location of the API key (header or query parameter).\"\
  \n    },\n    \"api-key-value\": {\n      \"type\": \"string\",\n      \"description\": \"Default value for the API key.\"\n    },\n    \"server-url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Default server URL to use for API requests.\"\n    },\n    \"default-api-server\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the default API server from the servers list.\"\n    },\n    \"fetch-credentials\": {\n      \"type\": \"string\",\n      \"enum\": [\"omit\", \"same-origin\", \"include\"],\n      \"default\": \"same-origin\",\n      \"description\": \"Credentials policy for fetch requests made from the Try It console.\"\n    },\n    \"match-type\": {\n      \"type\": \"string\",\n      \"enum\": [\"includes\", \"regex\"],\n      \"default\": \"includes\",\n      \"description\": \"Search match type for filtering endpoints.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rapidoc/refs/heads/main/json-schema/rapidoc-configuration.json
tags:
- Documentation
- Platform
- Web Components
- OpenAPI
title: RapiDoc Web Component Configuration
---
