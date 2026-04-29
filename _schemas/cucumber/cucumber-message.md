---
description: Subset schema for Cucumber Messages, the standard interchange format emitted by Cucumber implementations and consumed by formatters and reporters. See https://github.com/cucumber/messages for the canonical schema.
layout: schema
name: CucumberMessage
properties_list:
- description: ''
  name: meta
  type: object
- description: ''
  name: source
  type: object
- description: ''
  name: gherkinDocument
  type: object
- description: ''
  name: pickle
  type: object
- description: ''
  name: testRunStarted
  type: object
- description: ''
  name: testRunFinished
  type: object
- description: ''
  name: testCaseStarted
  type: object
- description: ''
  name: testCaseFinished
  type: object
- description: ''
  name: testStepStarted
  type: object
- description: ''
  name: testStepFinished
  type: object
- description: ''
  name: attachment
  type: object
provider_name: Cucumber
provider_slug: cucumber
schema_file: json-schema/cucumber-message-schema.json
slug: cucumber-message
source_filename: cucumber-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cucumber/refs/heads/main/json-schema/cucumber-message-schema.json\",\n  \"title\": \"CucumberMessage\",\n  \"description\": \"Subset schema for Cucumber Messages, the standard interchange format emitted by Cucumber implementations and consumed by formatters and reporters. See https://github.com/cucumber/messages for the canonical schema.\",\n  \"type\": \"object\",\n  \"oneOf\": [\n    {\"required\": [\"meta\"]},\n    {\"required\": [\"source\"]},\n    {\"required\": [\"gherkinDocument\"]},\n    {\"required\": [\"pickle\"]},\n    {\"required\": [\"testCaseStarted\"]},\n    {\"required\": [\"testCaseFinished\"]},\n    {\"required\": [\"testStepStarted\"]},\n    {\"required\": [\"testStepFinished\"]},\n    {\"required\": [\"testRunStarted\"]},\n    {\"required\": [\"testRunFinished\"]},\n    {\"required\": [\"attachment\"]}\n  ],\n  \"properties\"\
  : {\n    \"meta\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"protocolVersion\": {\"type\": \"string\"},\n        \"implementation\": {\"type\": \"object\", \"properties\": {\"name\": {\"type\": \"string\"}, \"version\": {\"type\": \"string\"}}},\n        \"runtime\": {\"type\": \"object\", \"properties\": {\"name\": {\"type\": \"string\"}, \"version\": {\"type\": \"string\"}}}\n      }\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"required\": [\"uri\", \"data\", \"mediaType\"],\n      \"properties\": {\n        \"uri\": {\"type\": \"string\"},\n        \"data\": {\"type\": \"string\"},\n        \"mediaType\": {\"type\": \"string\"}\n      }\n    },\n    \"gherkinDocument\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"uri\": {\"type\": \"string\"},\n        \"feature\": {\"$ref\": \"#/$defs/Feature\"},\n        \"comments\": {\"type\": \"array\", \"items\": {\"type\": \"object\"}}\n      }\n    },\n    \"pickle\": {\n  \
  \    \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\"type\": \"string\"},\n        \"uri\": {\"type\": \"string\"},\n        \"name\": {\"type\": \"string\"},\n        \"language\": {\"type\": \"string\"},\n        \"tags\": {\"type\": \"array\", \"items\": {\"type\": \"object\", \"properties\": {\"name\": {\"type\": \"string\"}}}},\n        \"steps\": {\"type\": \"array\", \"items\": {\"type\": \"object\"}}\n      }\n    },\n    \"testRunStarted\": {\"type\": \"object\", \"properties\": {\"timestamp\": {\"$ref\": \"#/$defs/Timestamp\"}}},\n    \"testRunFinished\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"success\": {\"type\": \"boolean\"},\n        \"timestamp\": {\"$ref\": \"#/$defs/Timestamp\"},\n        \"message\": {\"type\": \"string\"}\n      }\n    },\n    \"testCaseStarted\": {\"type\": \"object\"},\n    \"testCaseFinished\": {\"type\": \"object\"},\n    \"testStepStarted\": {\"type\": \"object\"},\n    \"testStepFinished\": {\n   \
  \   \"type\": \"object\",\n      \"properties\": {\n        \"testStepResult\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"status\": {\"type\": \"string\", \"enum\": [\"UNKNOWN\", \"PASSED\", \"SKIPPED\", \"PENDING\", \"UNDEFINED\", \"AMBIGUOUS\", \"FAILED\"]},\n            \"duration\": {\"type\": \"object\"},\n            \"message\": {\"type\": \"string\"}\n          }\n        }\n      }\n    },\n    \"attachment\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"body\": {\"type\": \"string\"},\n        \"contentEncoding\": {\"type\": \"string\", \"enum\": [\"IDENTITY\", \"BASE64\"]},\n        \"mediaType\": {\"type\": \"string\"},\n        \"fileName\": {\"type\": \"string\"}\n      }\n    }\n  },\n  \"$defs\": {\n    \"Timestamp\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"seconds\": {\"type\": \"integer\"},\n        \"nanos\": {\"type\": \"integer\"}\n      }\n    },\n    \"Feature\": {\n      \"type\"\
  : \"object\",\n      \"properties\": {\n        \"name\": {\"type\": \"string\"},\n        \"description\": {\"type\": \"string\"},\n        \"language\": {\"type\": \"string\"},\n        \"keyword\": {\"type\": \"string\"},\n        \"tags\": {\"type\": \"array\", \"items\": {\"type\": \"object\"}},\n        \"children\": {\"type\": \"array\", \"items\": {\"type\": \"object\"}}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cucumber/refs/heads/main/json-schema/cucumber-message-schema.json
tags:
- Automation
- BDD
- Behavior Driven Development
- Gherkin
- Open Source
- Quality Assurance
- Test Framework
- Testing
title: CucumberMessage
---
