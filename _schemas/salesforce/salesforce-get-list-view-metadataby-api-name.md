---
description: ''
layout: schema
name: GetListViewMetadatabyAPIName
properties_list:
- description: ''
  name: cloneable
  type: boolean
- description: ''
  name: createable
  type: boolean
- description: ''
  name: deletable
  type: boolean
- description: ''
  name: displayColumns
  type: array
- description: ''
  name: filterLogicString
  type: '[''string'', ''null'']'
- description: ''
  name: filteredByInfo
  type: array
- description: ''
  name: hasMassActions
  type: boolean
- description: ''
  name: inlineEditDetails
  type: object
- description: ''
  name: label
  type: string
- description: ''
  name: listReference
  type: object
- description: ''
  name: listShares
  type: object
- description: ''
  name: objectApiNames
  type: array
- description: ''
  name: orderedByInfo
  type: array
- description: ''
  name: scope
  type: object
- description: ''
  name: updateable
  type: boolean
- description: ''
  name: userPreferences
  type: object
- description: ''
  name: visibility
  type: string
- description: ''
  name: visibilityEditable
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-list-view-metadataby-api-name-schema.json
slug: salesforce-get-list-view-metadataby-api-name
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"cloneable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"createable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"deletable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"displayColumns\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldApiName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"inlineEditAttributes\": {\n            \"type\": \"object\",\n            \"example\": \"example_value\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"lookupId\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"500123\"\n          },\n\
  \          \"searchable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"sortable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          }\n        },\n        \"required\": [\n          \"fieldApiName\",\n          \"inlineEditAttributes\",\n          \"label\",\n          \"lookupId\",\n          \"searchable\",\n          \"sortable\"\n        ]\n      }\n    },\n    \"filterLogicString\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"filteredByInfo\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"hasMassActions\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"inlineEditDetails\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"Example Title\"\n    },\n    \"listReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"listViewApiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"objectApiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"listViewApiName\",\n        \"objectApiName\",\n        \"type\"\n      ]\n    },\n    \"listShares\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"objectApiNames\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"orderedByInfo\": {\n     \
  \ \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldApiName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"isAscending\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          }\n        },\n        \"required\": [\n          \"fieldApiName\",\n          \"isAscending\",\n          \"label\"\n        ]\n      }\n    },\n    \"scope\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"updateable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"userPreferences\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"columnWidths\": {\n          \"type\": \"object\",\n          \"properties\": {\n\
  \            \"Site\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            },\n            \"Type\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            },\n            \"BillingCountry\": {\n              \"type\": \"integer\",\n              \"example\": 42\n            },\n            \"Owner.Alias\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            },\n            \"Phone\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            },\n            \"Name\": {\n              \"type\": \"integer\",\n              \"example\": \"Example Title\"\n            }\n          },\n          \"required\": [\n            \"Site\",\n            \"Type\",\n            \"BillingCountry\",\n            \"Owner.Alias\",\n            \"Phone\",\n            \"Name\"\n          ]\n        },\n        \"columnWrap\": {\n          \"type\": \"object\",\n          \"properties\":\
  \ {\n            \"Site\": {\n              \"type\": \"boolean\",\n              \"example\": true\n            },\n            \"Type\": {\n              \"type\": \"boolean\",\n              \"example\": true\n            },\n            \"BillingCountry\": {\n              \"type\": \"boolean\",\n              \"example\": 42\n            },\n            \"Owner.Alias\": {\n              \"type\": \"boolean\",\n              \"example\": true\n            },\n            \"Phone\": {\n              \"type\": \"boolean\",\n              \"example\": true\n            },\n            \"Name\": {\n              \"type\": \"boolean\",\n              \"example\": \"Example Title\"\n            }\n          },\n          \"required\": [\n            \"Site\",\n            \"Type\",\n            \"BillingCountry\",\n            \"Owner.Alias\",\n            \"Phone\",\n            \"Name\"\n          ]\n        }\n      },\n      \"required\": [\n        \"columnWidths\",\n        \"columnWrap\"\
  \n      ]\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"visibilityEditable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"cloneable\",\n    \"createable\",\n    \"deletable\",\n    \"displayColumns\",\n    \"filterLogicString\",\n    \"filteredByInfo\",\n    \"hasMassActions\",\n    \"inlineEditDetails\",\n    \"label\",\n    \"listReference\",\n    \"listShares\",\n    \"objectApiNames\",\n    \"orderedByInfo\",\n    \"scope\",\n    \"updateable\",\n    \"userPreferences\",\n    \"visibility\",\n    \"visibilityEditable\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetListViewMetadatabyAPIName\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-list-view-metadataby-api-name-schema.json
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
title: GetListViewMetadatabyAPIName
---
