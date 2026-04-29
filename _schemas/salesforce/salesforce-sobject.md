---
description: A Salesforce SObject record as returned by the REST API. Contains an attributes object with type and URL metadata, an Id field with the 18-character record identifier, and dynamic fields specific to the object type (e.g., Name, Email, Phone for Contact).
layout: schema
name: Salesforce SObject Record
properties_list:
- description: ''
  name: attributes
  type: object
- description: The globally unique 18-character Salesforce record identifier. The first three characters are the key prefix identifying the object type, followed by a unique alphanumeric string.
  name: Id
  type: string
- description: The primary display name field for the record. For most standard objects this is the Name field; for Person Accounts and Contacts it may be a combination of first and last name.
  name: Name
  type:
  - string
  - 'null'
- description: The date and time the record was created, in ISO 8601 format with UTC timezone (e.g., 2024-01-15T10:30:00.000+0000).
  name: CreatedDate
  type:
  - string
  - 'null'
- description: The 18-character ID of the Salesforce user who created this record.
  name: CreatedById
  type:
  - string
  - 'null'
- description: The date and time the record was last modified, in ISO 8601 format with UTC timezone.
  name: LastModifiedDate
  type:
  - string
  - 'null'
- description: The 18-character ID of the Salesforce user who last modified this record.
  name: LastModifiedById
  type:
  - string
  - 'null'
- description: The date and time of the last system-level modification to the record. This is updated by any change to the record including system changes, unlike LastModifiedDate which reflects user changes only.
  name: SystemModstamp
  type:
  - string
  - 'null'
- description: Whether the record has been moved to the Recycle Bin (soft deleted). Records where IsDeleted is true are not returned by standard SOQL queries but can be retrieved using queryAll.
  name: IsDeleted
  type:
  - boolean
  - 'null'
- description: The 18-character ID of the user or queue that owns this record. Ownership controls access and assignment rules.
  name: OwnerId
  type:
  - string
  - 'null'
- description: The 18-character ID of the Record Type applied to this record. Record types allow different picklist values, page layouts, and business processes for the same object.
  name: RecordTypeId
  type:
  - string
  - 'null'
- description: The billing address for account records. A structured address object with street, city, state, postal code, country, and optional geolocation fields.
  name: BillingAddress
  type: object
- description: The shipping address for account records. A structured address object with street, city, state, postal code, country, and optional geolocation fields.
  name: ShippingAddress
  type: object
- description: The mailing address for contact records. A structured address object with street, city, state, postal code, country, and optional geolocation fields.
  name: MailingAddress
  type: object
- description: An alternate address for contact records. A structured address object with street, city, state, postal code, country, and optional geolocation fields.
  name: OtherAddress
  type: object
- description: The primary phone number for the record. Stored as a string to preserve formatting; no specific format is enforced by Salesforce.
  name: Phone
  type: object
- description: The fax number for the record. Stored as a string to preserve formatting.
  name: Fax
  type: object
- description: The mobile phone number for contact and lead records. Stored as a string to preserve formatting.
  name: MobilePhone
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-sobject-schema.json
slug: salesforce-sobject
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-sobject-schema.json\",\n  \"title\": \"Salesforce SObject Record\",\n  \"description\": \"A Salesforce SObject record as returned by the REST API. Contains an attributes object with type and URL metadata, an Id field with the 18-character record identifier, and dynamic fields specific to the object type (e.g., Name, Email, Phone for Contact).\",\n  \"type\": \"object\",\n  \"required\": [\n    \"attributes\"\n  ],\n  \"properties\": {\n    \"attributes\": {\n      \"$ref\": \"#/$defs/SObjectAttributes\"\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The globally unique 18-character Salesforce record identifier. The first three characters are the key prefix identifying the object type, followed by a unique alphanumeric string.\",\n      \"minLength\": 15,\n      \"maxLength\"\
  : 18,\n      \"pattern\": \"^[a-zA-Z0-9]{15,18}$\"\n    },\n    \"Name\": {\n      \"type\": [\n        \"string\",\n        \"null\"\n      ],\n      \"description\": \"The primary display name field for the record. For most standard objects this is the Name field; for Person Accounts and Contacts it may be a combination of first and last name.\"\n    },\n    \"CreatedDate\": {\n      \"type\": [\n        \"string\",\n        \"null\"\n      ],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was created, in ISO 8601 format with UTC timezone (e.g., 2024-01-15T10:30:00.000+0000).\"\n    },\n    \"CreatedById\": {\n      \"type\": [\n        \"string\",\n        \"null\"\n      ],\n      \"description\": \"The 18-character ID of the Salesforce user who created this record.\",\n      \"minLength\": 15,\n      \"maxLength\": 18\n    },\n    \"LastModifiedDate\": {\n      \"type\": [\n        \"string\",\n        \"null\"\n      ],\n      \"format\"\
  : \"date-time\",\n      \"description\": \"The date and time the record was last modified, in ISO 8601 format with UTC timezone.\"\n    },\n    \"LastModifiedById\": {\n      \"type\": [\n        \"string\",\n        \"null\"\n      ],\n      \"description\": \"The 18-character ID of the Salesforce user who last modified this record.\",\n      \"minLength\": 15,\n      \"maxLength\": 18\n    },\n    \"SystemModstamp\": {\n      \"type\": [\n        \"string\",\n        \"null\"\n      ],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the last system-level modification to the record. This is updated by any change to the record including system changes, unlike LastModifiedDate which reflects user changes only.\"\n    },\n    \"IsDeleted\": {\n      \"type\": [\n        \"boolean\",\n        \"null\"\n      ],\n      \"description\": \"Whether the record has been moved to the Recycle Bin (soft deleted). Records where IsDeleted is true are not returned by\
  \ standard SOQL queries but can be retrieved using queryAll.\"\n    },\n    \"OwnerId\": {\n      \"type\": [\n        \"string\",\n        \"null\"\n      ],\n      \"description\": \"The 18-character ID of the user or queue that owns this record. Ownership controls access and assignment rules.\",\n      \"minLength\": 15,\n      \"maxLength\": 18\n    },\n    \"RecordTypeId\": {\n      \"type\": [\n        \"string\",\n        \"null\"\n      ],\n      \"description\": \"The 18-character ID of the Record Type applied to this record. Record types allow different picklist values, page layouts, and business processes for the same object.\",\n      \"minLength\": 15,\n      \"maxLength\": 18\n    },\n    \"BillingAddress\": {\n      \"$ref\": \"#/$defs/Address\",\n      \"description\": \"The billing address for account records. A structured address object with street, city, state, postal code, country, and optional geolocation fields.\"\n    },\n    \"ShippingAddress\": {\n      \"$ref\"\
  : \"#/$defs/Address\",\n      \"description\": \"The shipping address for account records. A structured address object with street, city, state, postal code, country, and optional geolocation fields.\"\n    },\n    \"MailingAddress\": {\n      \"$ref\": \"#/$defs/Address\",\n      \"description\": \"The mailing address for contact records. A structured address object with street, city, state, postal code, country, and optional geolocation fields.\"\n    },\n    \"OtherAddress\": {\n      \"$ref\": \"#/$defs/Address\",\n      \"description\": \"An alternate address for contact records. A structured address object with street, city, state, postal code, country, and optional geolocation fields.\"\n    },\n    \"Phone\": {\n      \"$ref\": \"#/$defs/Phone\",\n      \"description\": \"The primary phone number for the record. Stored as a string to preserve formatting; no specific format is enforced by Salesforce.\"\n    },\n    \"Fax\": {\n      \"$ref\": \"#/$defs/Phone\",\n      \"description\"\
  : \"The fax number for the record. Stored as a string to preserve formatting.\"\n    },\n    \"MobilePhone\": {\n      \"$ref\": \"#/$defs/Phone\",\n      \"description\": \"The mobile phone number for contact and lead records. Stored as a string to preserve formatting.\"\n    }\n  },\n  \"additionalProperties\": true,\n  \"$defs\": {\n    \"SObjectAttributes\": {\n      \"type\": \"object\",\n      \"title\": \"SObject Attributes\",\n      \"description\": \"Metadata attributes included with every Salesforce SObject record, identifying the object type and the REST API URL for the record.\",\n      \"required\": [\n        \"type\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The API name of the Salesforce SObject type (e.g., Account, Contact, Opportunity, MyCustomObject__c). This identifies what kind of record this is.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\
  ,\n          \"description\": \"The relative REST API URL for this specific record (e.g., /services/data/v63.0/sobjects/Account/001Dn00000pFakE001). Use this URL to retrieve or update the record via the REST API.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"RecordType\": {\n      \"type\": \"object\",\n      \"title\": \"Record Type\",\n      \"description\": \"A Salesforce Record Type, which allows different picklist values, page layouts, and business processes to be configured for the same object type.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The 18-character ID of the Record Type.\",\n          \"minLength\": 15,\n          \"maxLength\": 18\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the Record Type (e.g., Business Account, Person Account).\"\n        },\n        \"active\": {\n          \"type\": \"boolean\",\n\
  \          \"description\": \"Whether this Record Type is currently active. Inactive record types cannot be assigned to new records.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"Address\": {\n      \"type\": [\n        \"object\",\n        \"null\"\n      ],\n      \"title\": \"Address\",\n      \"description\": \"A structured Salesforce compound address field containing street, city, state, postal code, country, and optional geolocation components.\",\n      \"properties\": {\n        \"street\": {\n          \"type\": [\n            \"string\",\n            \"null\"\n          ],\n          \"description\": \"The street address, including house number, street name, and apartment or suite number. May contain newline characters for multi-line addresses.\"\n        },\n        \"city\": {\n          \"type\": [\n            \"string\",\n            \"null\"\n          ],\n          \"description\": \"The city component of the address.\"\n        },\n    \
  \    \"state\": {\n          \"type\": [\n            \"string\",\n            \"null\"\n          ],\n          \"description\": \"The state or province component of the address (e.g., CA, New York, Ontario).\"\n        },\n        \"postalCode\": {\n          \"type\": [\n            \"string\",\n            \"null\"\n          ],\n          \"description\": \"The postal or ZIP code component of the address.\"\n        },\n        \"country\": {\n          \"type\": [\n            \"string\",\n            \"null\"\n          ],\n          \"description\": \"The country component of the address. May be a full country name or ISO 3166-1 alpha-2 country code depending on org configuration.\"\n        },\n        \"stateCode\": {\n          \"type\": [\n            \"string\",\n            \"null\"\n          ],\n          \"description\": \"The ISO 3166-2 state/province code if state/country picklists are enabled in the org.\"\n        },\n        \"countryCode\": {\n          \"type\"\
  : [\n            \"string\",\n            \"null\"\n          ],\n          \"description\": \"The ISO 3166-1 alpha-2 country code if state/country picklists are enabled in the org (e.g., US, GB, DE).\"\n        },\n        \"latitude\": {\n          \"type\": [\n            \"number\",\n            \"null\"\n          ],\n          \"description\": \"The latitude component of the geolocation for this address, in decimal degrees. Populated automatically by Salesforce geocoding when enabled.\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"longitude\": {\n          \"type\": [\n            \"number\",\n            \"null\"\n          ],\n          \"description\": \"The longitude component of the geolocation for this address, in decimal degrees. Populated automatically by Salesforce geocoding when enabled.\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        },\n        \"geocodeAccuracy\": {\n          \"type\": [\n            \"string\"\
  ,\n            \"null\"\n          ],\n          \"description\": \"The accuracy level of the geocoded coordinates (e.g., Address, NearAddress, Block, Street, ExtendedZip, Zip, Neighborhood, City, County, State, Unknown).\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"Phone\": {\n      \"type\": [\n        \"string\",\n        \"null\"\n      ],\n      \"title\": \"Phone Number\",\n      \"description\": \"A telephone number stored as a string. Salesforce does not enforce a specific format; common formats include +1 (555) 123-4567, 555-123-4567, or +15551234567.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-sobject-schema.json
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
title: Salesforce SObject Record
---
