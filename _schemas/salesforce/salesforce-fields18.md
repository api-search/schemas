---
description: ''
layout: schema
name: Fields18
properties_list:
- description: ''
  name: AnnualRevenue
  type: object
- description: ''
  name: BillingCity
  type: object
- description: ''
  name: BillingCountry
  type: object
- description: ''
  name: BillingPostalCode
  type: object
- description: ''
  name: BillingState
  type: object
- description: ''
  name: BillingStreet
  type: object
- description: ''
  name: Industry
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: OwnerId
  type: object
- description: ''
  name: Parent
  type: object
- description: ''
  name: ParentId
  type: object
- description: ''
  name: Phone
  type: object
- description: ''
  name: PhotoUrl
  type: object
- description: ''
  name: Site
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Website
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-fields18-schema.json
slug: salesforce-fields18
source_filename: salesforce-fields18-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnnualRevenue\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"BillingCity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"BillingCountry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string',\
  \ 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"BillingPostalCode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"BillingState\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n       \
  \ }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"BillingStreet\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Industry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Name\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\"\
  : {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Owner\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"apiName\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"childRelationships\": {\n              \"type\": \"object\",\n              \"example\": \"example_value\"\n            },\n            \"eTag\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"fields\": {\n   \
  \           \"type\": \"object\",\n              \"properties\": {\n                \"Id\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                },\n                \"Name\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n         \
  \             \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"Id\",\n                \"Name\"\n              ]\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            },\n            \"lastModifiedById\": {\n              \"type\": \"string\",\n              \"example\": \"500123\"\n            },\n            \"lastModifiedDate\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"recordTypeId\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"500123\"\n            },\n            \"recordTypeInfo\": {\n              \"type\": \"['string',\
  \ 'null']\",\n              \"example\": \"example_value\"\n            },\n            \"systemModstamp\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"weakEtag\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            }\n          },\n          \"required\": [\n            \"apiName\",\n            \"childRelationships\",\n            \"eTag\",\n            \"fields\",\n            \"id\",\n            \"lastModifiedById\",\n            \"lastModifiedDate\",\n            \"recordTypeId\",\n            \"recordTypeInfo\",\n            \"systemModstamp\",\n            \"weakEtag\"\n          ]\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"OwnerId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n\
  \        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Parent\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"ParentId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"\
  displayValue\",\n        \"value\"\n      ]\n    },\n    \"Phone\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"PhotoUrl\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Site\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\"\
  ,\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Type\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Website\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\"\
  : [\n        \"displayValue\",\n        \"value\"\n      ]\n    }\n  },\n  \"required\": [\n    \"AnnualRevenue\",\n    \"BillingCity\",\n    \"BillingCountry\",\n    \"BillingPostalCode\",\n    \"BillingState\",\n    \"BillingStreet\",\n    \"Industry\",\n    \"Name\",\n    \"Owner\",\n    \"OwnerId\",\n    \"Parent\",\n    \"ParentId\",\n    \"Phone\",\n    \"PhotoUrl\",\n    \"Site\",\n    \"Type\",\n    \"Website\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Fields18\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-fields18-schema.json
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
title: Fields18
---
