---
description: ''
layout: schema
name: Fields11
properties_list:
- description: ''
  name: AnnualRevenue
  type: object
- description: ''
  name: City
  type: object
- description: ''
  name: Company
  type: object
- description: ''
  name: Country
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
  name: CurrentGenerators__c
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Email
  type: object
- description: ''
  name: Fax
  type: object
- description: ''
  name: FirstName
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
  name: LastName
  type: object
- description: ''
  name: LeadSource
  type: object
- description: ''
  name: MobilePhone
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
  name: Phone
  type: object
- description: ''
  name: PostalCode
  type: object
- description: ''
  name: Primary__c
  type: object
- description: ''
  name: ProductInterest__c
  type: object
- description: ''
  name: Rating
  type: object
- description: ''
  name: SICCode__c
  type: object
- description: ''
  name: Salutation
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Street
  type: object
- description: ''
  name: Title
  type: object
- description: ''
  name: Website
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-fields11-schema.json
slug: salesforce-fields11
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnnualRevenue\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"City\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Company\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\":\
  \ {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Country\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"CreatedBy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"object\",\n          \"properties\": {\n         \
  \   \"apiName\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"childRelationships\": {\n              \"type\": \"object\",\n              \"example\": \"example_value\"\n            },\n            \"eTag\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"fields\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Id\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\"\
  ,\n                    \"value\"\n                  ]\n                },\n                \"Name\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"Id\",\n                \"Name\"\n              ]\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            },\n            \"lastModifiedById\": {\n              \"type\": \"string\"\
  ,\n              \"example\": \"500123\"\n            },\n            \"lastModifiedDate\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"recordTypeId\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"500123\"\n            },\n            \"recordTypeInfo\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"example_value\"\n            },\n            \"systemModstamp\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"weakEtag\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            }\n          },\n          \"required\": [\n            \"apiName\",\n            \"childRelationships\",\n            \"eTag\",\n            \"fields\",\n            \"id\",\n            \"lastModifiedById\",\n            \"lastModifiedDate\",\n            \"recordTypeId\",\n \
  \           \"recordTypeInfo\",\n            \"systemModstamp\",\n            \"weakEtag\"\n          ]\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"CreatedById\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"CreatedDate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\
  \n      ]\n    },\n    \"CurrentGenerators__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Description\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Email\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\"\
  ,\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Fax\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"FirstName\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n  \
  \    \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Industry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"apiName\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"childRelationships\": {\n              \"type\": \"object\",\n           \
  \   \"example\": \"example_value\"\n            },\n            \"eTag\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"fields\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Id\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                },\n                \"Name\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n              \
  \      \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"Id\",\n                \"Name\"\n              ]\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            },\n            \"lastModifiedById\": {\n              \"type\": \"string\",\n              \"example\": \"500123\"\n            },\n            \"lastModifiedDate\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n\
  \            \"recordTypeId\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"500123\"\n            },\n            \"recordTypeInfo\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"example_value\"\n            },\n            \"systemModstamp\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"weakEtag\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            }\n          },\n          \"required\": [\n            \"apiName\",\n            \"childRelationships\",\n            \"eTag\",\n            \"fields\",\n            \"id\",\n            \"lastModifiedById\",\n            \"lastModifiedDate\",\n            \"recordTypeId\",\n            \"recordTypeInfo\",\n            \"systemModstamp\",\n            \"weakEtag\"\n          ]\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n\
  \      ]\n    },\n    \"LastModifiedById\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"LastName\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\"\
  : \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"LeadSource\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"MobilePhone\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n      \
  \  \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"NumberOfEmployees\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"NumberofLocations__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Owner\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n       \
  \   \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"apiName\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"childRelationships\": {\n              \"type\": \"object\",\n              \"example\": \"example_value\"\n            },\n            \"eTag\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"fields\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Id\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"\
  string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                },\n                \"Name\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"displayValue\": {\n                      \"type\": \"['string', 'null']\",\n                      \"example\": \"example_value\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"displayValue\",\n                    \"value\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"Id\",\n                \"Name\"\n              ]\n            },\n    \
  \        \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            },\n            \"lastModifiedById\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"500123\"\n            },\n            \"lastModifiedDate\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"example_value\"\n            },\n            \"recordTypeId\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"500123\"\n            },\n            \"recordTypeInfo\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"example_value\"\n            },\n            \"systemModstamp\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"example_value\"\n            },\n            \"weakEtag\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            }\n          },\n          \"required\": [\n            \"apiName\"\
  ,\n            \"childRelationships\",\n            \"eTag\",\n            \"fields\",\n            \"id\",\n            \"lastModifiedById\",\n            \"lastModifiedDate\",\n            \"recordTypeId\",\n            \"recordTypeInfo\",\n            \"systemModstamp\",\n            \"weakEtag\"\n          ]\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"OwnerId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Phone\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"\
  example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"PostalCode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Primary__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\"\
  ,\n        \"value\"\n      ]\n    },\n    \"ProductInterest__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Rating\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"SICCode__c\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string',\
  \ 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Salutation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"State\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\"\
  : [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Status\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Street\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Title\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"\
  ['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    },\n    \"Website\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayValue\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"value\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"displayValue\",\n        \"value\"\n      ]\n    }\n  },\n  \"required\": [\n    \"AnnualRevenue\",\n    \"City\",\n    \"Company\",\n    \"Country\",\n    \"CreatedBy\",\n    \"CreatedById\",\n    \"CreatedDate\",\n    \"CurrentGenerators__c\",\n    \"Description\",\n    \"Email\",\n    \"Fax\",\n    \"FirstName\",\n    \"Industry\",\n    \"LastModifiedBy\"\
  ,\n    \"LastModifiedById\",\n    \"LastModifiedDate\",\n    \"LastName\",\n    \"LeadSource\",\n    \"MobilePhone\",\n    \"NumberOfEmployees\",\n    \"NumberofLocations__c\",\n    \"Owner\",\n    \"OwnerId\",\n    \"Phone\",\n    \"PostalCode\",\n    \"Primary__c\",\n    \"ProductInterest__c\",\n    \"Rating\",\n    \"SICCode__c\",\n    \"Salutation\",\n    \"State\",\n    \"Status\",\n    \"Street\",\n    \"Title\",\n    \"Website\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Fields11\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-fields11-schema.json
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
title: Fields11
---
