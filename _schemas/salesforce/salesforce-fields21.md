---
description: ''
layout: schema
name: Fields21
properties_list:
- description: ''
  name: AccountNumber
  type: object
- description: ''
  name: Active__c
  type: object
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
  name: CreatedBy
  type: object
- description: ''
  name: CreatedById
  type: object
- description: ''
  name: CreatedDate
  type: object
- description: ''
  name: CustomerPriority__c
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Fax
  type: object
- description: ''
  name: Industry
  type: object
- description: ''
  name: LastModifiedBy
  type: object
- description: ''
  name: LastModifiedById
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: NumberOfEmployees
  type: object
- description: ''
  name: NumberofLocations__c
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: OwnerId
  type: object
- description: ''
  name: Ownership
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
  name: Rating
  type: object
- description: ''
  name: SLAExpirationDate__c
  type: object
- description: ''
  name: SLASerialNumber__c
  type: object
- description: ''
  name: SLA__c
  type: object
- description: ''
  name: ShippingCity
  type: object
- description: ''
  name: ShippingCountry
  type: object
- description: ''
  name: ShippingPostalCode
  type: object
- description: ''
  name: ShippingState
  type: object
- description: ''
  name: ShippingStreet
  type: object
- description: ''
  name: Sic
  type: object
- description: ''
  name: Site
  type: object
- description: ''
  name: TickerSymbol
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: UpsellOpportunity__c
  type: object
- description: ''
  name: Website
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-fields21-schema.json
slug: salesforce-fields21
source_filename: salesforce-fields21-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountNumber\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Active__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"AnnualRevenue\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\"\
  : {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"BillingCity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"BillingCountry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string',\
  \ 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"BillingPostalCode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"BillingState\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n  \
  \    ]\n    },\n    \"BillingStreet\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"CreatedBy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"apiName\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"childRelationships\": {\n              \"type\": \"object\",\n              \"example\": \"example_value\"\n            },\n            \"eTag\"\
  : {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"fields\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Id\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                },\n                \"Name\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\"\
  ,\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"Id\",\n                \"Name\"\n              ]\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            },\n            \"lastModifiedById\": {\n              \"type\": \"string\",\n              \"example\": \"500123\"\n            },\n            \"lastModifiedDate\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"recordTypeId\": {\n              \"type\": \"['string', 'null']\",\n\
  \              \"example\": \"500123\"\n            },\n            \"recordTypeInfo\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"example_value\"\n            },\n            \"systemModstamp\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"weakEtag\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            }\n          },\n          \"required\": [\n            \"apiName\",\n            \"childRelationships\",\n            \"eTag\",\n            \"fields\",\n            \"id\",\n            \"lastModifiedById\",\n            \"lastModifiedDate\",\n            \"recordTypeId\",\n            \"recordTypeInfo\",\n            \"systemModstamp\",\n            \"weakEtag\"\n          ]\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"CreatedById\": {\n      \"type\": \"object\",\n      \"properties\"\
  : {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"CreatedDate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"CustomerPriority__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string',\
  \ 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Description\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Fax\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n\
  \    \"Industry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"apiName\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"childRelationships\": {\n              \"type\": \"object\",\n              \"example\": \"example_value\"\n            },\n            \"eTag\": {\n        \
  \      \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"fields\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Id\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                },\n                \"Name\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n\
  \                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"Id\",\n                \"Name\"\n              ]\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            },\n            \"lastModifiedById\": {\n              \"type\": \"string\",\n              \"example\": \"500123\"\n            },\n            \"lastModifiedDate\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"recordTypeId\": {\n              \"type\": \"['string', 'null']\",\n  \
  \            \"example\": \"500123\"\n            },\n            \"recordTypeInfo\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"example_value\"\n            },\n            \"systemModstamp\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"weakEtag\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            }\n          },\n          \"required\": [\n            \"apiName\",\n            \"childRelationships\",\n            \"eTag\",\n            \"fields\",\n            \"id\",\n            \"lastModifiedById\",\n            \"lastModifiedDate\",\n            \"recordTypeId\",\n            \"recordTypeInfo\",\n            \"systemModstamp\",\n            \"weakEtag\"\n          ]\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"LastModifiedById\": {\n      \"type\": \"object\",\n      \"\
  properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Name\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\"\
  ,\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"NumberOfEmployees\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"NumberofLocations__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n     \
  \ ]\n    },\n    \"Owner\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"apiName\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"childRelationships\": {\n              \"type\": \"object\",\n              \"example\": \"example_value\"\n            },\n            \"eTag\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"fields\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Id\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\"\
  : \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                },\n                \"Name\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                }\n              },\n      \
  \        \"required\": [\n                \"Id\",\n                \"Name\"\n              ]\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            },\n            \"lastModifiedById\": {\n              \"type\": \"string\",\n              \"example\": \"500123\"\n            },\n            \"lastModifiedDate\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"recordTypeId\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"500123\"\n            },\n            \"recordTypeInfo\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"example_value\"\n            },\n            \"systemModstamp\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"weakEtag\": {\n              \"type\": \"integer\",\n              \"example\"\
  : 10\n            }\n          },\n          \"required\": [\n            \"apiName\",\n            \"childRelationships\",\n            \"eTag\",\n            \"fields\",\n            \"id\",\n            \"lastModifiedById\",\n            \"lastModifiedDate\",\n            \"recordTypeId\",\n            \"recordTypeInfo\",\n            \"systemModstamp\",\n            \"weakEtag\"\n          ]\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"OwnerId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Ownership\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"\
  displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Parent\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"ParentId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string',\
  \ 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Phone\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Rating\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n   \
  \ \"SLAExpirationDate__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"SLASerialNumber__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"SLA__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\"\
  ,\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"ShippingCity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"ShippingCountry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\
  \n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"ShippingPostalCode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"ShippingState\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"ShippingStreet\": {\n      \"type\"\
  : \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Sic\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Site\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n  \
  \      \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"TickerSymbol\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Type\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"\
  displayValue\",\n        \"value\"\n      ]\n    },\n    \"UpsellOpportunity__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Website\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountNumber\",\n    \"Active__c\",\n    \"AnnualRevenue\",\n    \"\
  BillingCity\",\n    \"BillingCountry\",\n    \"BillingPostalCode\",\n    \"BillingState\",\n    \"BillingStreet\",\n    \"CreatedBy\",\n    \"CreatedById\",\n    \"CreatedDate\",\n    \"CustomerPriority__c\",\n    \"Description\",\n    \"Fax\",\n    \"Industry\",\n    \"LastModifiedBy\",\n    \"LastModifiedById\",\n    \"LastModifiedDate\",\n    \"Name\",\n    \"NumberOfEmployees\",\n    \"NumberofLocations__c\",\n    \"Owner\",\n    \"OwnerId\",\n    \"Ownership\",\n    \"Parent\",\n    \"ParentId\",\n    \"Phone\",\n    \"Rating\",\n    \"SLAExpirationDate__c\",\n    \"SLASerialNumber__c\",\n    \"SLA__c\",\n    \"ShippingCity\",\n    \"ShippingCountry\",\n    \"ShippingPostalCode\",\n    \"ShippingState\",\n    \"ShippingStreet\",\n    \"Sic\",\n    \"Site\",\n    \"TickerSymbol\",\n    \"Type\",\n    \"UpsellOpportunity__c\",\n    \"Website\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Fields21\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-fields21-schema.json
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
title: Fields21
---
