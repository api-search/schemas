---
description: ''
layout: schema
name: LookupResults
properties_list:
- description: ''
  name: Account
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-lookup-results-schema.json
slug: salesforce-lookup-results
source_filename: salesforce-lookup-results-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Account\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"count\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        },\n        \"currentPageToken\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"CAUQAA\"\n        },\n        \"currentPageUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"nextPageToken\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"CAUQAA\"\n        },\n        \"nextPageUrl\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"previousPageToken\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"CAUQAA\"\n        },\n        \"previousPageUrl\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n  \
  \      },\n        \"records\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"apiName\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"childRelationships\": {\n                \"type\": \"object\",\n                \"example\": \"example_value\"\n              },\n              \"eTag\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"fields\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"Id\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"displayValue\": {\n                        \"type\": \"object\"\n                      },\n                      \"value\": {\n  \
  \                      \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"displayValue\",\n                      \"value\"\n                    ]\n                  },\n                  \"Name\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"displayValue\": {\n                        \"type\": \"object\"\n                      },\n                      \"value\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"displayValue\",\n                      \"value\"\n                    ]\n                  },\n                  \"Site\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"displayValue\": {\n                        \"type\": \"object\"\n                      },\n      \
  \                \"value\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"displayValue\",\n                      \"value\"\n                    ]\n                  }\n                },\n                \"required\": [\n                  \"Id\",\n                  \"Name\",\n                  \"Site\"\n                ]\n              },\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              },\n              \"lastModifiedById\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"lastModifiedDate\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"recordTypeId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n       \
  \       \"recordTypeInfo\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"example_value\"\n              },\n              \"systemModstamp\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"weakEtag\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              }\n            },\n            \"required\": [\n              \"apiName\",\n              \"childRelationships\",\n              \"eTag\",\n              \"fields\",\n              \"id\",\n              \"lastModifiedById\",\n              \"lastModifiedDate\",\n              \"recordTypeId\",\n              \"recordTypeInfo\",\n              \"systemModstamp\",\n              \"weakEtag\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"count\",\n        \"currentPageToken\",\n        \"currentPageUrl\",\n        \"nextPageToken\",\n        \"nextPageUrl\"\
  ,\n        \"previousPageToken\",\n        \"previousPageUrl\",\n        \"records\"\n      ]\n    }\n  },\n  \"required\": [\n    \"Account\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LookupResults\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-lookup-results-schema.json
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
title: LookupResults
---
