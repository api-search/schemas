---
description: DataFilter describes constraints and filters for event data.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.DataFilter
properties_list:
- description: Comparator compares the event data with a user given value. Can be ">=", ">", "=", "!=", "<", or "<=". Is optional, and if left blank treated as equality "=".
  name: comparator
  type: string
- description: Path is the JSONPath of the event's (JSON decoded) data key. Path is a series of keys separated by a dot. A key may contain wildcard characters '*' and '?'. To access an array value use the index as t
  name: path
  type: string
- description: ''
  name: template
  type: string
- description: ''
  name: type
  type: string
- description: Value is the allowed string values for this key. Booleans are parsed using strconv.ParseBool(), Numbers are parsed as float64 using strconv.ParseFloat(), Strings are treated as regular expressions, Ni
  name: value
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-data-filter-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-data-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-data-filter-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.DataFilter\",\n  \"description\": \"DataFilter describes constraints and filters for event data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comparator\": {\n      \"description\": \"Comparator compares the event data with a user given value.\\nCan be \\\">=\\\", \\\">\\\", \\\"=\\\", \\\"!=\\\", \\\"<\\\", or \\\"<=\\\".\\nIs optional, and if left blank treated as equality \\\"=\\\".\",\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"description\": \"Path is the JSONPath of the event's (JSON decoded) data key.\\nPath is a series of keys separated by a dot. A key may contain wildcard characters '*' and '?'.\\\
  nTo access an array value use the index as the key. The dot and wildcard characters can be escaped with '\\\\\\\\'.\\nSee https://github.com/tidwall/gjson#path-syntax for more information on how to use this.\",\n      \"type\": \"string\"\n    },\n    \"template\": {\n      \"type\": \"string\",\n      \"title\": \"Template is a go-template for extracting a string from the event's data.\\nA Template is evaluated with provided path, type and value.\\nThe templating follows the standard go-template syntax as well as sprig's extra functions.\\nSee https://pkg.go.dev/text/template and https://masterminds.github.io/sprig/\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"title\": \"Type contains the JSON type of the data\"\n    },\n    \"value\": {\n      \"description\": \"Value is the allowed string values for this key.\\nBooleans are parsed using strconv.ParseBool(),\\nNumbers are parsed as float64 using strconv.ParseFloat(),\\nStrings are treated as regular expressions,\\\
  nNils value is ignored.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-data-filter-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.DataFilter
---
