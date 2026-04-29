---
description: ''
layout: schema
name: SymbolTable
properties_list:
- description: ''
  name: constructors
  type: array
- description: ''
  name: externalReferences
  type: array
- description: ''
  name: id
  type: string
- description: ''
  name: innerClasses
  type: array
- description: ''
  name: interfaces
  type: array
- description: ''
  name: key
  type: string
- description: ''
  name: methods
  type: array
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: parentClass
  type: string
- description: ''
  name: properties
  type: array
- description: ''
  name: tableDeclaration
  type: object
- description: ''
  name: variables
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-symbol-table-schema.json
slug: salesforce-symbol-table
source_filename: salesforce-symbol-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"constructors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"annotations\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"location\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"column\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              },\n              \"line\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              }\n            },\n            \"required\": [\n              \"column\",\n              \"line\"\n            ]\n          },\n          \"modifiers\": {\n            \"type\": \"array\",\n            \"description\"\
  : \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"parameters\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"example\": \"Example Title\"\n                },\n                \"type\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"name\",\n                \"type\"\n              ]\n            }\n          },\n          \"references\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n  \
  \          \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"type\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"annotations\",\n          \"location\",\n          \"modifiers\",\n          \"name\",\n          \"parameters\",\n          \"references\",\n          \"type\"\n        ]\n      }\n    },\n    \"externalReferences\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"innerClasses\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"interfaces\": {\n      \"type\": \"array\",\n      \"description\": \"\"\
  ,\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"methods\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"annotations\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"location\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"column\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              },\n              \"line\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              }\n            },\n            \"required\": [\n              \"column\",\n           \
  \   \"line\"\n            ]\n          },\n          \"modifiers\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"parameters\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"example\": \"Example Title\"\n                },\n                \"type\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"name\",\n                \"type\"\n              ]\n\
  \            }\n          },\n          \"references\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"returnType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"type\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"annotations\",\n          \"location\",\n          \"modifiers\",\n          \"name\",\n          \"parameters\",\n          \"references\",\n          \"returnType\",\n          \"type\"\n        ]\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"parentClass\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"example_value\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tableDeclaration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"annotations\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              }\n            },\n            \"required\": [\n              \"name\"\n            ]\n          }\n        },\n        \"location\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"column\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            },\n            \"line\": {\n              \"type\"\
  : \"integer\",\n              \"example\": 10\n            }\n          },\n          \"required\": [\n            \"column\",\n            \"line\"\n          ]\n        },\n        \"modifiers\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"references\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"annotations\",\n        \"location\",\n        \"modifiers\",\n        \"name\",\n        \"references\",\n        \"type\"\n      ]\n    },\n    \"variables\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"constructors\",\n    \"externalReferences\",\n    \"id\",\n    \"innerClasses\",\n    \"interfaces\",\n    \"key\",\n    \"methods\",\n    \"name\",\n    \"namespace\",\n    \"parentClass\",\n    \"properties\",\n    \"tableDeclaration\",\n    \"variables\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SymbolTable\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-symbol-table-schema.json
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
title: SymbolTable
---
