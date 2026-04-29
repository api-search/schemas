---
description: A paginated list of reports.
layout: schema
name: paginated_reports
properties_list:
- description: Page number of the current results. This is an optional element that is not provided in all responses.
  name: page
  type: integer
- description: The values of the current page.
  name: values
  type: array
- description: Total number of objects in the response. This is an optional element that is not provided in all responses, as it can be expensive to compute.
  name: size
  type: integer
- description: Current number of objects on the existing page. The default value is 10 with 100 being the maximum allowed value. Individual APIs may enforce different values.
  name: pagelen
  type: integer
- description: Link to the next page if it exists. The last page of a collection does not have this value. Use this link to navigate the result set and refrain from constructing your own URLs.
  name: next
  type: string
- description: Link to previous page if it exists. A collections first page does not have this value. This is an optional element that is not provided in all responses. Some result sets strictly support forward navi
  name: previous
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-paginated_reports-schema.json
slug: atlassian-bitbucket-repositories-paginated_reports
source_filename: atlassian-bitbucket-repositories-paginated_reports-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"paginated_reports\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of reports.\",\n  \"properties\": {\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Page number of the current results. This is an optional element that is not provided in all responses.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"The values of the current page.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of objects in the response. This is an optional element that is not provided in all responses, as it can be expensive to compute.\"\n    },\n    \"pagelen\": {\n      \"type\": \"integer\",\n      \"description\": \"Current number of objects on the existing page. The default value is 10 with 100 being the maximum allowed value. Individual APIs may enforce different values.\"\n    },\n    \"next\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Link to the next page if it exists. The last page of a collection does not have this value. Use this link to navigate the result set and refrain from constructing your own URLs.\"\n    },\n    \"previous\": {\n      \"type\": \"string\",\n      \"description\": \"Link to previous page if it exists. A collections first page does not have this value. This is an optional element that is not provided in all responses. Some result sets strictly support forward navigation and never provide previous links. Clients must anticipate that backwards navigation is not always available. Use this link to navigate the result set and refrain from constructing your own URLs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-paginated_reports-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: paginated_reports
---
