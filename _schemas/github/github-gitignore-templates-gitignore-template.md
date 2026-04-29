---
description: Gitignore Template
layout: schema
name: gitignore-template
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: source
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-gitignore-templates-gitignore-template-schema.json
slug: github-gitignore-templates-gitignore-template
source_filename: github-gitignore-templates-gitignore-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-gitignore-templates-gitignore-template-schema.json\",\n  \"title\": \"gitignore-template\",\n  \"description\": \"Gitignore Template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"C\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"example\": \"# Object files\\n*.o\\n\\n# Libraries\\n*.lib\\n*.a\\n\\n# Shared objects (inc. Windows DLLs)\\n*.dll\\n*.so\\n*.so.*\\n*.dylib\\n\\n# Executables\\n*.exe\\n*.out\\n*.app\\n\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-gitignore-templates-gitignore-template-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: gitignore-template
---
