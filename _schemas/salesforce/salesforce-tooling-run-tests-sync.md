---
description: ''
layout: schema
name: ToolingRunTestsSync
properties_list:
- description: ''
  name: apexLogId
  type: string
- description: ''
  name: codeCoverage
  type: array
- description: ''
  name: codeCoverageWarnings
  type: array
- description: ''
  name: failures
  type: array
- description: ''
  name: flowCoverage
  type: array
- description: ''
  name: flowCoverageWarnings
  type: array
- description: ''
  name: numFailures
  type: integer
- description: ''
  name: numTestsRun
  type: integer
- description: ''
  name: successes
  type: array
- description: ''
  name: totalTime
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-tooling-run-tests-sync-schema.json
slug: salesforce-tooling-run-tests-sync
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"apexLogId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"codeCoverage\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"locationsNotCovered\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\"\n            }\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"namespace\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"numLocations\": {\n            \"type\": \"integer\",\n           \
  \ \"example\": 10\n          },\n          \"numLocationsNotCovered\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"locationsNotCovered\",\n          \"name\",\n          \"namespace\",\n          \"numLocations\",\n          \"numLocationsNotCovered\",\n          \"type\"\n        ]\n      }\n    },\n    \"codeCoverageWarnings\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"name\": {\n            \"type\": \"['string',\
  \ 'null']\",\n            \"example\": \"Example Title\"\n          },\n          \"namespace\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"message\",\n          \"name\",\n          \"namespace\"\n        ]\n      }\n    },\n    \"failures\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"flowCoverage\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"flowCoverageWarnings\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"numFailures\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"numTestsRun\": {\n      \"\
  type\": \"integer\",\n      \"example\": 10\n    },\n    \"successes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"methodName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"namespace\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"seeAllData\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"time\": {\n            \"type\": \"integer\",\n            \"example\": 1700000000000\n          }\n        },\n        \"required\": [\n          \"id\",\n        \
  \  \"methodName\",\n          \"name\",\n          \"namespace\",\n          \"seeAllData\",\n          \"time\"\n        ]\n      }\n    },\n    \"totalTime\": {\n      \"type\": \"integer\",\n      \"example\": 1700000000000\n    }\n  },\n  \"required\": [\n    \"apexLogId\",\n    \"codeCoverage\",\n    \"codeCoverageWarnings\",\n    \"failures\",\n    \"flowCoverage\",\n    \"flowCoverageWarnings\",\n    \"numFailures\",\n    \"numTestsRun\",\n    \"successes\",\n    \"totalTime\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ToolingRunTestsSync\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-tooling-run-tests-sync-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: ToolingRunTestsSync
---
