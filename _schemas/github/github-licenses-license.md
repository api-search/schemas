---
description: License
layout: schema
name: license
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: spdx_id
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: node_id
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: implementation
  type: string
- description: ''
  name: permissions
  type: array
- description: ''
  name: conditions
  type: array
- description: ''
  name: limitations
  type: array
- description: ''
  name: body
  type: string
- description: ''
  name: featured
  type: boolean
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-licenses-license-schema.json
slug: github-licenses-license
source_filename: github-licenses-license-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-licenses-license-schema.json\",\n  \"title\": \"license\",\n  \"description\": \"License\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"example\": \"mit\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"MIT License\"\n    },\n    \"spdx_id\": {\n      \"type\": \"string\",\n      \"example\": \"MIT\",\n      \"nullable\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/licenses/mit\",\n      \"nullable\": true\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDc6TGljZW5zZW1pdA==\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://choosealicense.com/licenses/mit/\"\
  \n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A permissive license that is short and to the point. It lets people do anything with your code with proper attribution and without warranty.\"\n    },\n    \"implementation\": {\n      \"type\": \"string\",\n      \"example\": \"Create a text file (typically named LICENSE or LICENSE.txt) in the root of your source code and copy the text of the license into the file. Replace [year] with the current year and [fullname] with the name (or names) of the copyright holders.\"\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"example\": [\n        \"commercial-use\",\n        \"modifications\",\n        \"distribution\",\n        \"sublicense\",\n        \"private-use\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"conditions\": {\n      \"type\": \"array\",\n      \"example\": [\n        \"include-copyright\"\n      ],\n      \"items\": {\n        \"type\"\
  : \"string\"\n      }\n    },\n    \"limitations\": {\n      \"type\": \"array\",\n      \"example\": [\n        \"no-liability\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"example\": \"\\n\\nThe MIT License (MIT)\\n\\nCopyright (c) [year] [fullname]\\n\\nPermission is hereby granted, free of charge, to any person obtaining a copy\\nof this software and associated documentation files (the \\\"Software\\\"), to deal\\nin the Software without restriction, including without limitation the rights\\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\\ncopies of the Software, and to permit persons to whom the Software is\\nfurnished to do so, subject to the following conditions:\\n\\nThe above copyright notice and this permission notice shall be included in all\\ncopies or substantial portions of the Software.\\n\\nTHE SOFTWARE IS PROVIDED \\\"AS IS\\\", WITHOUT WARRANTY OF ANY KIND,\
  \ EXPRESS OR\\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\\nSOFTWARE.\\n\"\n    },\n    \"featured\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"name\",\n    \"url\",\n    \"spdx_id\",\n    \"node_id\",\n    \"html_url\",\n    \"description\",\n    \"implementation\",\n    \"permissions\",\n    \"conditions\",\n    \"limitations\",\n    \"body\",\n    \"featured\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-licenses-license-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: license
---
