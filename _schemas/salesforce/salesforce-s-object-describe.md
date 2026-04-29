---
description: ''
layout: schema
name: SObjectDescribe
properties_list:
- description: ''
  name: actionOverrides
  type: array
- description: ''
  name: activateable
  type: boolean
- description: ''
  name: associateEntityType
  type: '[''string'', ''null'']'
- description: ''
  name: associateParentEntity
  type: '[''string'', ''null'']'
- description: ''
  name: childRelationships
  type: array
- description: ''
  name: compactLayoutable
  type: boolean
- description: ''
  name: createable
  type: boolean
- description: ''
  name: custom
  type: boolean
- description: ''
  name: customSetting
  type: boolean
- description: ''
  name: deepCloneable
  type: boolean
- description: ''
  name: defaultImplementation
  type: '[''string'', ''null'']'
- description: ''
  name: deletable
  type: boolean
- description: ''
  name: deprecatedAndHidden
  type: boolean
- description: ''
  name: extendedBy
  type: '[''string'', ''null'']'
- description: ''
  name: extendsInterfaces
  type: '[''string'', ''null'']'
- description: ''
  name: feedEnabled
  type: boolean
- description: ''
  name: fields
  type: array
- description: ''
  name: hasSubtypes
  type: boolean
- description: ''
  name: implementedBy
  type: '[''string'', ''null'']'
- description: ''
  name: implementsInterfaces
  type: '[''string'', ''null'']'
- description: ''
  name: isInterface
  type: boolean
- description: ''
  name: isSubtype
  type: boolean
- description: ''
  name: keyPrefix
  type: string
- description: ''
  name: label
  type: string
- description: ''
  name: labelPlural
  type: string
- description: ''
  name: layoutable
  type: boolean
- description: ''
  name: listviewable
  type: '[''string'', ''null'']'
- description: ''
  name: lookupLayoutable
  type: '[''string'', ''null'']'
- description: ''
  name: mergeable
  type: boolean
- description: ''
  name: mruEnabled
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: namedLayoutInfos
  type: array
- description: ''
  name: networkScopeFieldName
  type: '[''string'', ''null'']'
- description: ''
  name: queryable
  type: boolean
- description: ''
  name: recordTypeInfos
  type: array
- description: ''
  name: replicateable
  type: boolean
- description: ''
  name: retrieveable
  type: boolean
- description: ''
  name: searchLayoutable
  type: boolean
- description: ''
  name: searchable
  type: boolean
- description: ''
  name: sobjectDescribeOption
  type: string
- description: ''
  name: supportedScopes
  type: array
- description: ''
  name: triggerable
  type: boolean
- description: ''
  name: undeletable
  type: boolean
- description: ''
  name: updateable
  type: boolean
- description: ''
  name: urls
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-s-object-describe-schema.json
slug: salesforce-s-object-describe
source_filename: salesforce-s-object-describe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionOverrides\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"formFactor\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"isAvailableInTouch\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"pageId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"url\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"https://www.example.com\"\n          }\n        },\n        \"required\": [\n          \"formFactor\",\n          \"isAvailableInTouch\",\n          \"name\",\n          \"pageId\",\n    \
  \      \"url\"\n        ]\n      }\n    },\n    \"activateable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"associateEntityType\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"associateParentEntity\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"childRelationships\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"cascadeDelete\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"childSObject\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"deprecatedAndHidden\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"field\": {\n            \"type\": \"string\",\n            \"example\"\
  : \"example_value\"\n          },\n          \"junctionIdListNames\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"junctionReferenceTo\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"relationshipName\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"restrictedDelete\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          }\n        },\n        \"required\": [\n          \"cascadeDelete\",\n          \"childSObject\",\n          \"deprecatedAndHidden\",\n          \"field\",\n          \"junctionIdListNames\",\n          \"junctionReferenceTo\",\n          \"relationshipName\"\
  ,\n          \"restrictedDelete\"\n        ]\n      }\n    },\n    \"compactLayoutable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"createable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"custom\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"customSetting\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"deepCloneable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"defaultImplementation\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"deletable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"deprecatedAndHidden\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"extendedBy\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"extendsInterfaces\": {\n      \"type\": \"['string', 'null']\",\n      \"example\"\
  : \"example_value\"\n    },\n    \"feedEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"aggregatable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"aiPredictionField\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"autoNumber\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"byteLength\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"calculated\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"calculatedFormula\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n      \
  \    \"cascadeDelete\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"caseSensitive\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"compoundFieldName\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"controllerName\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"createable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"custom\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"defaultValue\": {\n            \"type\": \"object\",\n            \"example\": \"example_value\"\n          },\n          \"defaultValueFormula\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"defaultedOnCreate\"\
  : {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"dependentPicklist\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"deprecatedAndHidden\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"digits\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"displayLocationInDecimal\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"encrypted\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"externalId\": {\n            \"type\": \"boolean\",\n            \"example\": \"500123\"\n          },\n          \"extraTypeInfo\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"filterable\": {\n            \"type\": \"boolean\",\n            \"example\"\
  : true\n          },\n          \"filteredLookupInfo\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"formulaTreatNullNumberAsZero\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"groupable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"highScaleNumber\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"htmlFormatted\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"idLookup\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"inlineHelpText\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n       \
  \   \"length\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"mask\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"maskType\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"nameField\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"namePointing\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"nillable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"permissionable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"picklistValues\": {\n            \"type\": \"array\",\n            \"description\"\
  : \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\"\n            }\n          },\n          \"polymorphicForeignKey\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"precision\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"queryByDistance\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"referenceTargetField\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"referenceTo\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"relationshipName\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"relationshipOrder\"\
  : {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"restrictedDelete\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"restrictedPicklist\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"scale\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"searchPrefilterable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"soapType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"sortable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"unique\": {\n            \"type\": \"boolean\",\n            \"example\": true\n\
  \          },\n          \"updateable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"writeRequiresMasterRead\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          }\n        },\n        \"required\": [\n          \"aggregatable\",\n          \"aiPredictionField\",\n          \"autoNumber\",\n          \"byteLength\",\n          \"calculated\",\n          \"calculatedFormula\",\n          \"cascadeDelete\",\n          \"caseSensitive\",\n          \"compoundFieldName\",\n          \"controllerName\",\n          \"createable\",\n          \"custom\",\n          \"defaultValue\",\n          \"defaultValueFormula\",\n          \"defaultedOnCreate\",\n          \"dependentPicklist\",\n          \"deprecatedAndHidden\",\n          \"digits\",\n          \"displayLocationInDecimal\",\n          \"encrypted\",\n          \"externalId\",\n          \"extraTypeInfo\",\n          \"filterable\",\n          \"filteredLookupInfo\"\
  ,\n          \"formulaTreatNullNumberAsZero\",\n          \"groupable\",\n          \"highScaleNumber\",\n          \"htmlFormatted\",\n          \"idLookup\",\n          \"inlineHelpText\",\n          \"label\",\n          \"length\",\n          \"mask\",\n          \"maskType\",\n          \"name\",\n          \"nameField\",\n          \"namePointing\",\n          \"nillable\",\n          \"permissionable\",\n          \"picklistValues\",\n          \"polymorphicForeignKey\",\n          \"precision\",\n          \"queryByDistance\",\n          \"referenceTargetField\",\n          \"referenceTo\",\n          \"relationshipName\",\n          \"relationshipOrder\",\n          \"restrictedDelete\",\n          \"restrictedPicklist\",\n          \"scale\",\n          \"searchPrefilterable\",\n          \"soapType\",\n          \"sortable\",\n          \"type\",\n          \"unique\",\n          \"updateable\",\n          \"writeRequiresMasterRead\"\n        ]\n      }\n    },\n    \"hasSubtypes\"\
  : {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"implementedBy\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"implementsInterfaces\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"isInterface\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"isSubtype\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"keyPrefix\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"labelPlural\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"layoutable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"listviewable\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"lookupLayoutable\": {\n      \"type\"\
  : \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"mergeable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"mruEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"namedLayoutInfos\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"networkScopeFieldName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"queryable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"recordTypeInfos\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"active\": {\n            \"type\": \"boolean\",\n            \"example\": true\n\
  \          },\n          \"available\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"defaultRecordTypeMapping\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"developerName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"master\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"recordTypeId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"urls\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"layout\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"layout\"\
  \n            ]\n          }\n        },\n        \"required\": [\n          \"active\",\n          \"available\",\n          \"defaultRecordTypeMapping\",\n          \"developerName\",\n          \"master\",\n          \"name\",\n          \"recordTypeId\",\n          \"urls\"\n        ]\n      }\n    },\n    \"replicateable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"retrieveable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"searchLayoutable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"searchable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"sobjectDescribeOption\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"supportedScopes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"label\": {\n            \"type\"\
  : \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          }\n        },\n        \"required\": [\n          \"label\",\n          \"name\"\n        ]\n      }\n    },\n    \"triggerable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"undeletable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"updateable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"urls\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"compactLayouts\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"rowTemplate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"approvalLayouts\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"uiDetailTemplate\"\
  : {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"uiEditTemplate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"listviews\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"describe\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"uiNewRecord\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"quickActions\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"layouts\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"sobject\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"compactLayouts\",\n        \"rowTemplate\",\n        \"approvalLayouts\"\
  ,\n        \"uiDetailTemplate\",\n        \"uiEditTemplate\",\n        \"listviews\",\n        \"describe\",\n        \"uiNewRecord\",\n        \"quickActions\",\n        \"layouts\",\n        \"sobject\"\n      ]\n    }\n  },\n  \"required\": [\n    \"actionOverrides\",\n    \"activateable\",\n    \"associateEntityType\",\n    \"associateParentEntity\",\n    \"childRelationships\",\n    \"compactLayoutable\",\n    \"createable\",\n    \"custom\",\n    \"customSetting\",\n    \"deepCloneable\",\n    \"defaultImplementation\",\n    \"deletable\",\n    \"deprecatedAndHidden\",\n    \"extendedBy\",\n    \"extendsInterfaces\",\n    \"feedEnabled\",\n    \"fields\",\n    \"hasSubtypes\",\n    \"implementedBy\",\n    \"implementsInterfaces\",\n    \"isInterface\",\n    \"isSubtype\",\n    \"keyPrefix\",\n    \"label\",\n    \"labelPlural\",\n    \"layoutable\",\n    \"listviewable\",\n    \"lookupLayoutable\",\n    \"mergeable\",\n    \"mruEnabled\",\n    \"name\",\n    \"namedLayoutInfos\"\
  ,\n    \"networkScopeFieldName\",\n    \"queryable\",\n    \"recordTypeInfos\",\n    \"replicateable\",\n    \"retrieveable\",\n    \"searchLayoutable\",\n    \"searchable\",\n    \"sobjectDescribeOption\",\n    \"supportedScopes\",\n    \"triggerable\",\n    \"undeletable\",\n    \"updateable\",\n    \"urls\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SObjectDescribe\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-s-object-describe-schema.json
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
title: SObjectDescribe
---
