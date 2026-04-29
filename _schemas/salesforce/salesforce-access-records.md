---
description: ''
layout: schema
name: AccessRecords
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: Id
  type: string
- description: ''
  name: NamespacePrefix
  type: string
- description: ''
  name: Name
  type: string
- description: ''
  name: ApiVersion
  type: integer
- description: ''
  name: Status
  type: string
- description: ''
  name: IsValid
  type: boolean
- description: ''
  name: BodyCrc
  type: integer
- description: ''
  name: Body
  type: string
- description: ''
  name: LengthWithoutComments
  type: integer
- description: ''
  name: CreatedDate
  type: string
- description: ''
  name: CreatedById
  type: string
- description: ''
  name: LastModifiedDate
  type: string
- description: ''
  name: LastModifiedById
  type: string
- description: ''
  name: SystemModstamp
  type: string
- description: ''
  name: ManageableState
  type: string
- description: ''
  name: SymbolTable
  type: object
- description: ''
  name: Metadata
  type: object
- description: ''
  name: FullName
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-access-records-schema.json
slug: salesforce-access-records
source_filename: salesforce-access-records-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"url\"\n      ]\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"NamespacePrefix\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"ApiVersion\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"IsValid\": {\n      \"type\": \"boolean\",\n      \"example\": \"500123\"\n    },\n    \"\
  BodyCrc\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"Body\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"LengthWithoutComments\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"ManageableState\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"SymbolTable\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"constructors\": {\n          \"type\": \"array\",\n \
  \         \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"annotations\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"location\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"column\": {\n                    \"type\": \"integer\",\n                    \"example\": 10\n                  },\n                  \"line\": {\n                    \"type\": \"integer\",\n                    \"example\": 10\n                  }\n                },\n                \"required\": [\n                  \"column\",\n                  \"line\"\n                ]\n              },\n              \"modifiers\": {\n                \"type\": \"array\",\n \
  \               \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"parameters\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"name\": {\n                      \"type\": \"object\"\n                    },\n                    \"type\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"name\",\n                    \"type\"\n                  ]\n                }\n              },\n              \"references\": {\n                \"type\"\
  : \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"type\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"annotations\",\n              \"location\",\n              \"modifiers\",\n              \"name\",\n              \"parameters\",\n              \"references\",\n              \"type\"\n            ]\n          }\n        },\n        \"externalReferences\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"innerClasses\": {\n          \"type\": \"array\",\n  \
  \        \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"interfaces\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"methods\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"annotations\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"location\": {\n                \"type\": \"object\",\n             \
  \   \"properties\": {\n                  \"column\": {\n                    \"type\": \"integer\",\n                    \"example\": 10\n                  },\n                  \"line\": {\n                    \"type\": \"integer\",\n                    \"example\": 10\n                  }\n                },\n                \"required\": [\n                  \"column\",\n                  \"line\"\n                ]\n              },\n              \"modifiers\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"parameters\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n\
  \                  \"type\": \"object\",\n                  \"properties\": {\n                    \"name\": {\n                      \"type\": \"object\"\n                    },\n                    \"type\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"name\",\n                    \"type\"\n                  ]\n                }\n              },\n              \"references\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"returnType\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"type\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"example_value\"\n              }\n          \
  \  },\n            \"required\": [\n              \"annotations\",\n              \"location\",\n              \"modifiers\",\n              \"name\",\n              \"parameters\",\n              \"references\",\n              \"returnType\",\n              \"type\"\n            ]\n          }\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"parentClass\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"properties\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"tableDeclaration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"annotations\": {\n              \"type\":\
  \ \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"example\": \"Example Title\"\n                  }\n                },\n                \"required\": [\n                  \"name\"\n                ]\n              }\n            },\n            \"location\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"column\": {\n                  \"type\": \"integer\",\n                  \"example\": 10\n                },\n                \"line\": {\n                  \"type\": \"integer\",\n                  \"example\": 10\n                }\n              },\n              \"required\": [\n                \"column\",\n                \"line\"\n              ]\n            },\n            \"modifiers\": {\n              \"\
  type\": \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"example\": \"Example Title\"\n            },\n            \"references\": {\n              \"type\": \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"type\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"annotations\",\n            \"location\",\n            \"modifiers\",\n            \"name\",\n            \"references\",\n            \"type\"\n          ]\n        },\n        \"variables\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"\
  example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\n        \"constructors\",\n        \"externalReferences\",\n        \"id\",\n        \"innerClasses\",\n        \"interfaces\",\n        \"key\",\n        \"methods\",\n        \"name\",\n        \"namespace\",\n        \"parentClass\",\n        \"properties\",\n        \"tableDeclaration\",\n        \"variables\"\n      ]\n    },\n    \"Metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apiVersion\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"packageVersions\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"urls\": {\n          \"type\":\
  \ \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"apiVersion\",\n        \"packageVersions\",\n        \"status\",\n        \"urls\"\n      ]\n    },\n    \"FullName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"attributes\",\n    \"Id\",\n    \"NamespacePrefix\",\n    \"Name\",\n    \"ApiVersion\",\n    \"Status\",\n    \"IsValid\",\n    \"BodyCrc\",\n    \"Body\",\n    \"LengthWithoutComments\",\n    \"CreatedDate\",\n    \"CreatedById\",\n    \"LastModifiedDate\",\n    \"LastModifiedById\",\n    \"SystemModstamp\",\n    \"ManageableState\",\n    \"SymbolTable\",\n    \"Metadata\",\n    \"FullName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessRecords\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-access-records-schema.json
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
title: AccessRecords
---
