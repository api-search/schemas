---
description: ''
layout: schema
name: Fields4
properties_list:
- description: ''
  name: Address
  type: object
- description: ''
  name: AnnualRevenue
  type: object
- description: ''
  name: City
  type: object
- description: ''
  name: CleanStatus
  type: object
- description: ''
  name: CloneSourceId
  type: object
- description: ''
  name: Company
  type: object
- description: ''
  name: CompanyDunsNumber
  type: object
- description: ''
  name: ConvertedAccountId
  type: object
- description: ''
  name: ConvertedContactId
  type: object
- description: ''
  name: ConvertedDate
  type: object
- description: ''
  name: ConvertedOpportunityId
  type: object
- description: ''
  name: Country
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
  name: DandbCompanyId
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Email
  type: object
- description: ''
  name: EmailBouncedDate
  type: object
- description: ''
  name: EmailBouncedReason
  type: object
- description: ''
  name: Fax
  type: object
- description: ''
  name: FirstName
  type: object
- description: ''
  name: GeocodeAccuracy
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: IndividualId
  type: object
- description: ''
  name: Industry
  type: object
- description: ''
  name: IsConverted
  type: object
- description: ''
  name: IsDeleted
  type: object
- description: ''
  name: IsUnreadByOwner
  type: object
- description: ''
  name: Jigsaw
  type: object
- description: ''
  name: JigsawContactId
  type: object
- description: ''
  name: LastActivityDate
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
  name: LastReferencedDate
  type: object
- description: ''
  name: LastViewedDate
  type: object
- description: ''
  name: Latitude
  type: object
- description: ''
  name: LeadSource
  type: object
- description: ''
  name: Longitude
  type: object
- description: ''
  name: MasterRecordId
  type: object
- description: ''
  name: MobilePhone
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
  name: OwnerId
  type: object
- description: ''
  name: Phone
  type: object
- description: ''
  name: PhotoUrl
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
  name: SystemModstamp
  type: object
- description: ''
  name: Title
  type: object
- description: ''
  name: Website
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-fields4-schema.json
slug: salesforce-fields4
source_filename: salesforce-fields4-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"calculated\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compound\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compoundComponentName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"compoundFieldName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllerName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllingFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n\
  \            \"type\": \"string\"\n          }\n        },\n        \"createable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"custom\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"extraTypeInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"filterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"filteredLookupInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"highScaleNumber\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"htmlFormatted\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"inlineHelpText\": {\n          \"type\":\
  \ \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"nameField\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"polymorphicForeignKey\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"precision\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"reference\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"referenceTargetField\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"referenceToInfos\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"\
  type\": \"string\"\n          }\n        },\n        \"relationshipName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"scale\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"searchPrefilterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"sortable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"unique\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"updateable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"apiName\",\n        \"calculated\",\n        \"compound\",\n        \"compoundComponentName\",\n        \"compoundFieldName\",\n        \"controllerName\",\n        \"controllingFields\"\
  ,\n        \"createable\",\n        \"custom\",\n        \"dataType\",\n        \"extraTypeInfo\",\n        \"filterable\",\n        \"filteredLookupInfo\",\n        \"highScaleNumber\",\n        \"htmlFormatted\",\n        \"inlineHelpText\",\n        \"label\",\n        \"length\",\n        \"nameField\",\n        \"polymorphicForeignKey\",\n        \"precision\",\n        \"reference\",\n        \"referenceTargetField\",\n        \"referenceToInfos\",\n        \"relationshipName\",\n        \"required\",\n        \"scale\",\n        \"searchPrefilterable\",\n        \"sortable\",\n        \"unique\",\n        \"updateable\"\n      ]\n    },\n    \"AnnualRevenue\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"calculated\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compound\": {\n          \"type\": \"boolean\"\
  ,\n          \"example\": true\n        },\n        \"compoundComponentName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"compoundFieldName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllerName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllingFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"createable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"custom\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"extraTypeInfo\": {\n  \
  \        \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"filterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"filteredLookupInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"highScaleNumber\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"htmlFormatted\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"inlineHelpText\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"nameField\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"polymorphicForeignKey\"\
  : {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"precision\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"reference\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"referenceTargetField\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"referenceToInfos\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"relationshipName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"scale\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"searchPrefilterable\": {\n          \"\
  type\": \"boolean\",\n          \"example\": true\n        },\n        \"sortable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"unique\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"updateable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"apiName\",\n        \"calculated\",\n        \"compound\",\n        \"compoundComponentName\",\n        \"compoundFieldName\",\n        \"controllerName\",\n        \"controllingFields\",\n        \"createable\",\n        \"custom\",\n        \"dataType\",\n        \"extraTypeInfo\",\n        \"filterable\",\n        \"filteredLookupInfo\",\n        \"highScaleNumber\",\n        \"htmlFormatted\",\n        \"inlineHelpText\",\n        \"label\",\n        \"length\",\n        \"nameField\",\n        \"polymorphicForeignKey\",\n        \"precision\",\n        \"reference\",\n        \"referenceTargetField\"\
  ,\n        \"referenceToInfos\",\n        \"relationshipName\",\n        \"required\",\n        \"scale\",\n        \"searchPrefilterable\",\n        \"sortable\",\n        \"unique\",\n        \"updateable\"\n      ]\n    },\n    \"City\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"calculated\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compound\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compoundComponentName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"compoundFieldName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"controllerName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllingFields\"\
  : {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"createable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"custom\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"extraTypeInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"filterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"filteredLookupInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"highScaleNumber\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"htmlFormatted\": {\n   \
  \       \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"inlineHelpText\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"nameField\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"polymorphicForeignKey\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"precision\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"reference\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"referenceTargetField\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"referenceToInfos\": {\n        \
  \  \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"relationshipName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"scale\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"searchPrefilterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"sortable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"unique\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"updateable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"apiName\",\n        \"calculated\",\n        \"compound\"\
  ,\n        \"compoundComponentName\",\n        \"compoundFieldName\",\n        \"controllerName\",\n        \"controllingFields\",\n        \"createable\",\n        \"custom\",\n        \"dataType\",\n        \"extraTypeInfo\",\n        \"filterable\",\n        \"filteredLookupInfo\",\n        \"highScaleNumber\",\n        \"htmlFormatted\",\n        \"inlineHelpText\",\n        \"label\",\n        \"length\",\n        \"nameField\",\n        \"polymorphicForeignKey\",\n        \"precision\",\n        \"reference\",\n        \"referenceTargetField\",\n        \"referenceToInfos\",\n        \"relationshipName\",\n        \"required\",\n        \"scale\",\n        \"searchPrefilterable\",\n        \"sortable\",\n        \"unique\",\n        \"updateable\"\n      ]\n    },\n    \"CleanStatus\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"calculated\": {\n \
  \         \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compound\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compoundComponentName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"compoundFieldName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllerName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllingFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"createable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"custom\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"dataType\"\
  : {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"extraTypeInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"filterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"filteredLookupInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"highScaleNumber\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"htmlFormatted\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"inlineHelpText\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"example\": 10\n       \
  \ },\n        \"nameField\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"polymorphicForeignKey\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"precision\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"reference\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"referenceTargetField\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"referenceToInfos\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"relationshipName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n \
  \       \"scale\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"searchPrefilterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"sortable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"unique\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"updateable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"apiName\",\n        \"calculated\",\n        \"compound\",\n        \"compoundComponentName\",\n        \"compoundFieldName\",\n        \"controllerName\",\n        \"controllingFields\",\n        \"createable\",\n        \"custom\",\n        \"dataType\",\n        \"extraTypeInfo\",\n        \"filterable\",\n        \"filteredLookupInfo\",\n        \"highScaleNumber\",\n        \"htmlFormatted\",\n        \"inlineHelpText\",\n        \"label\",\n\
  \        \"length\",\n        \"nameField\",\n        \"polymorphicForeignKey\",\n        \"precision\",\n        \"reference\",\n        \"referenceTargetField\",\n        \"referenceToInfos\",\n        \"relationshipName\",\n        \"required\",\n        \"scale\",\n        \"searchPrefilterable\",\n        \"sortable\",\n        \"unique\",\n        \"updateable\"\n      ]\n    },\n    \"CloneSourceId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"calculated\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compound\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compoundComponentName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"compoundFieldName\": {\n          \"type\": \"['string', 'null']\",\n \
  \         \"example\": \"example_value\"\n        },\n        \"controllerName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllingFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"createable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"custom\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"extraTypeInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"filterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"filteredLookupInfo\": {\n          \"type\": \"['string',\
  \ 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"highScaleNumber\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"htmlFormatted\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"inlineHelpText\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"nameField\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"polymorphicForeignKey\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"precision\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"reference\": {\n          \"type\": \"boolean\",\n          \"\
  example\": true\n        },\n        \"referenceTargetField\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"referenceToInfos\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"relationshipName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"scale\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"searchPrefilterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"sortable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"unique\": {\n          \"type\": \"boolean\",\n          \"example\": true\n\
  \        },\n        \"updateable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"apiName\",\n        \"calculated\",\n        \"compound\",\n        \"compoundComponentName\",\n        \"compoundFieldName\",\n        \"controllerName\",\n        \"controllingFields\",\n        \"createable\",\n        \"custom\",\n        \"dataType\",\n        \"extraTypeInfo\",\n        \"filterable\",\n        \"filteredLookupInfo\",\n        \"highScaleNumber\",\n        \"htmlFormatted\",\n        \"inlineHelpText\",\n        \"label\",\n        \"length\",\n        \"nameField\",\n        \"polymorphicForeignKey\",\n        \"precision\",\n        \"reference\",\n        \"referenceTargetField\",\n        \"referenceToInfos\",\n        \"relationshipName\",\n        \"required\",\n        \"scale\",\n        \"searchPrefilterable\",\n        \"sortable\",\n        \"unique\",\n        \"updateable\"\n      ]\n    },\n   \
  \ \"Company\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"calculated\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compound\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compoundComponentName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"compoundFieldName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllerName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllingFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n   \
  \     \"createable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"custom\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"extraTypeInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"filterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"filteredLookupInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"highScaleNumber\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"htmlFormatted\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"inlineHelpText\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\
  \n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"nameField\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"polymorphicForeignKey\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"precision\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"reference\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"referenceTargetField\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"referenceToInfos\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"relationshipName\"\
  : {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"scale\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"searchPrefilterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"sortable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"unique\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"updateable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"apiName\",\n        \"calculated\",\n        \"compound\",\n        \"compoundComponentName\",\n        \"compoundFieldName\",\n        \"controllerName\",\n        \"controllingFields\",\n        \"createable\",\n        \"custom\",\n        \"dataType\"\
  ,\n        \"extraTypeInfo\",\n        \"filterable\",\n        \"filteredLookupInfo\",\n        \"highScaleNumber\",\n        \"htmlFormatted\",\n        \"inlineHelpText\",\n        \"label\",\n        \"length\",\n        \"nameField\",\n        \"polymorphicForeignKey\",\n        \"precision\",\n        \"reference\",\n        \"referenceTargetField\",\n        \"referenceToInfos\",\n        \"relationshipName\",\n        \"required\",\n        \"scale\",\n        \"searchPrefilterable\",\n        \"sortable\",\n        \"unique\",\n        \"updateable\"\n      ]\n    },\n    \"CompanyDunsNumber\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"calculated\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compound\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compoundComponentName\"\
  : {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"compoundFieldName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllerName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllingFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"createable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"custom\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"extraTypeInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\
  \n        },\n        \"filterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"filteredLookupInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"highScaleNumber\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"htmlFormatted\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"inlineHelpText\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"nameField\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"polymorphicForeignKey\": {\n          \"type\": \"boolean\",\n          \"example\": true\n\
  \        },\n        \"precision\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"reference\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"referenceTargetField\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"referenceToInfos\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"relationshipName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"scale\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"searchPrefilterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n  \
  \      \"sortable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"unique\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"updateable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"apiName\",\n        \"calculated\",\n        \"compound\",\n        \"compoundComponentName\",\n        \"compoundFieldName\",\n        \"controllerName\",\n        \"controllingFields\",\n        \"createable\",\n        \"custom\",\n        \"dataType\",\n        \"extraTypeInfo\",\n        \"filterable\",\n        \"filteredLookupInfo\",\n        \"highScaleNumber\",\n        \"htmlFormatted\",\n        \"inlineHelpText\",\n        \"label\",\n        \"length\",\n        \"nameField\",\n        \"polymorphicForeignKey\",\n        \"precision\",\n        \"reference\",\n        \"referenceTargetField\",\n        \"referenceToInfos\",\n        \"relationshipName\"\
  ,\n        \"required\",\n        \"scale\",\n        \"searchPrefilterable\",\n        \"sortable\",\n        \"unique\",\n        \"updateable\"\n      ]\n    },\n    \"ConvertedAccountId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"apiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"calculated\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compound\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"compoundComponentName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"compoundFieldName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllerName\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"controllingFields\": {\n  \
  \        \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"createable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"custom\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"extraTypeInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"filterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"filteredLookupInfo\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"highScaleNumber\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"htmlFormatted\": {\n         \
  \ \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"inlineHelpText\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"nameField\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"polymorphicForeignKey\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"precision\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"reference\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"referenceTargetField\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"referenceToInfos\": {\n          \"type\"\
  : \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"apiName\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"nameFields\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            \"required\": [\n              \"apiName\",\n              \"nameFields\"\n            ]\n          }\n        },\n        \"relationshipName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"scale\": {\n          \"type\": \"integer\",\n          \"example\": 10\n \
  \       },\n        \"searchPrefilterable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"sortable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"unique\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"updateable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"apiName\",\n        \"calculated\",\n        \"compound\",\n        \"compoundComponentName\",\n        \"compoundFieldName\",\n        \"controllerName\",\n        \"controllingFields\",\n        \"createable\",\n        \"custom\",\n        \"dataType\",\n        \"extraTypeInfo\",\n        \"filterable\",\n        \"filteredLookupInfo\",\n        \"highScaleNumber\",\n        \"htmlFormatted\",\n        \"inlineHelpText\",\n        \"label\",\n        \"length\",\n        \"nameField\",\n \n\n# --- truncated at 32 KB (243 KB total)\
  \ ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-fields4-schema.json\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-fields4-schema.json
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
title: Fields4
---
