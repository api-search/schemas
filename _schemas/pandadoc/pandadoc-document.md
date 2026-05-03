---
description: Schema representing a PandaDoc document throughout its lifecycle, from initial draft through sending, signing, and completion. Documents are the central entity in PandaDoc and can be created from templates, uploaded files, or remote URLs.
layout: schema
name: PandaDoc Document
properties_list:
- description: Unique identifier assigned to the document by PandaDoc.
  name: id
  type: string
- description: Display name of the document as shown in the PandaDoc workspace.
  name: name
  type: string
- description: ''
  name: status
  type: object
- description: ISO 8601 timestamp indicating when the document was first created.
  name: date_created
  type: string
- description: ISO 8601 timestamp indicating when the document was last modified.
  name: date_modified
  type: string
- description: ISO 8601 timestamp after which the document expires and can no longer be signed. Null if no expiration is set.
  name: expiration_date
  type:
  - string
  - 'null'
- description: Document version string, incremented when the document is resent or edited.
  name: version
  type:
  - string
  - 'null'
- description: UUID assigned to the document, used as an alternative identifier in some contexts.
  name: uuid
  type:
  - string
  - 'null'
- description: List of string tags applied to the document for categorization and filtering.
  name: tags
  type: array
- description: Identifier of the folder where this document is stored.
  name: folder_uuid
  type:
  - string
  - 'null'
- description: The PandaDoc user who created the document.
  name: created_by
  type: object
- description: The PandaDoc user who sent the document for signature. Null if the document has not yet been sent.
  name: sent_by
  type: object
- description: List of recipients assigned to the document who may be required to sign, approve, or receive a copy.
  name: recipients
  type: array
- description: Reference to the PandaDoc template this document was generated from. Null if the document was created from a file upload.
  name: template
  type: object
- description: Total monetary value of all pricing table line items in the document. Null if the document contains no pricing tables.
  name: grand_total
  type: object
- description: Arbitrary key-value pairs attached to the document by the integrating application. Useful for storing external system references such as CRM IDs.
  name: metadata
  type: object
- description: List of CRM or external system objects linked to this document.
  name: linked_objects
  type: array
provider_name: PandaDoc
provider_slug: pandadoc
schema_file: json-schema/pandadoc-document-schema.json
slug: pandadoc-document
source_filename: pandadoc-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://pandadoc.com/schemas/pandadoc/document.json\",\n  \"title\": \"PandaDoc Document\",\n  \"description\": \"Schema representing a PandaDoc document throughout its lifecycle, from initial draft through sending, signing, and completion. Documents are the central entity in PandaDoc and can be created from templates, uploaded files, or remote URLs.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned to the document by PandaDoc.\",\n      \"example\": \"cKbJ7uay3cEGtsKuGPwYGX\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the document as shown in the PandaDoc workspace.\",\n      \"minLength\": 1,\n      \"maxLength\": 255,\n      \"example\": \"Service Agreement Q1 2026\"\n    },\n    \"status\": {\n\
  \      \"$ref\": \"#/$defs/DocumentStatus\"\n    },\n    \"date_created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp indicating when the document was first created.\"\n    },\n    \"date_modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp indicating when the document was last modified.\"\n    },\n    \"expiration_date\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp after which the document expires and can no longer be signed. Null if no expiration is set.\"\n    },\n    \"version\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Document version string, incremented when the document is resent or edited.\"\n    },\n    \"uuid\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uuid\",\n      \"description\": \"UUID assigned to the document,\
  \ used as an alternative identifier in some contexts.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"List of string tags applied to the document for categorization and filtering.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"folder_uuid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Identifier of the folder where this document is stored.\",\n      \"example\": \"BhVzRcxH9Z2LgfPPGXFUBa\"\n    },\n    \"created_by\": {\n      \"$ref\": \"#/$defs/UserReference\",\n      \"description\": \"The PandaDoc user who created the document.\"\n    },\n    \"sent_by\": {\n      \"oneOf\": [\n        {\"$ref\": \"#/$defs/UserReference\"},\n        {\"type\": \"null\"}\n      ],\n      \"description\": \"The PandaDoc user who sent the document for signature. Null if the document has not yet been sent.\"\n    },\n    \"recipients\": {\n      \"type\": \"array\",\n      \"description\": \"List of recipients assigned\
  \ to the document who may be required to sign, approve, or receive a copy.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Recipient\"\n      }\n    },\n    \"template\": {\n      \"oneOf\": [\n        {\"$ref\": \"#/$defs/TemplateReference\"},\n        {\"type\": \"null\"}\n      ],\n      \"description\": \"Reference to the PandaDoc template this document was generated from. Null if the document was created from a file upload.\"\n    },\n    \"grand_total\": {\n      \"oneOf\": [\n        {\"$ref\": \"#/$defs/MonetaryAmount\"},\n        {\"type\": \"null\"}\n      ],\n      \"description\": \"Total monetary value of all pricing table line items in the document. Null if the document contains no pricing tables.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Arbitrary key-value pairs attached to the document by the integrating application. Useful for storing external system references such as CRM IDs.\",\n      \"additionalProperties\": {\n   \
  \     \"type\": \"string\"\n      }\n    },\n    \"linked_objects\": {\n      \"type\": \"array\",\n      \"description\": \"List of CRM or external system objects linked to this document.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LinkedObject\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"DocumentStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Lifecycle status of a PandaDoc document. Documents progress through statuses as they move through the signing workflow.\",\n      \"enum\": [\n        \"document.draft\",\n        \"document.sent\",\n        \"document.completed\",\n        \"document.uploaded\",\n        \"document.error\",\n        \"document.viewed\",\n        \"document.waiting_approval\",\n        \"document.approved\",\n        \"document.rejected\",\n        \"document.waiting_pay\",\n        \"document.paid\",\n        \"document.voided\",\n        \"document.declined\",\n        \"document.external_review\"\n      ],\n      \"example\": \"document.draft\"\
  \n    },\n    \"UserReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a PandaDoc user account.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the PandaDoc user.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address of the user.\"\n        },\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\": \"First name of the user.\"\n        },\n        \"last_name\": {\n          \"type\": \"string\",\n          \"description\": \"Last name of the user.\"\n        },\n        \"avatar\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"URL of the user's profile avatar image.\"\n        },\n        \"membership_id\": {\n          \"type\": \"string\",\n          \"description\": \"Workspace membership\
  \ identifier for the user.\"\n        }\n      }\n    },\n    \"Recipient\": {\n      \"type\": \"object\",\n      \"description\": \"A person assigned to a document who may be required to sign, approve, or receive a copy.\",\n      \"required\": [\"id\", \"recipient_type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Participant classification.\",\n          \"const\": \"recipient\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the recipient within the document.\"\n        },\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\": \"First name of the recipient.\"\n        },\n        \"last_name\": {\n          \"type\": \"string\",\n          \"description\": \"Last name of the recipient.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"\
  Email address of the recipient.\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number of the recipient.\"\n        },\n        \"recipient_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of participation required from this recipient.\",\n          \"enum\": [\"SIGNER\", \"CC\", \"APPROVER\"]\n        },\n        \"role\": {\n          \"type\": \"string\",\n          \"description\": \"Role name that maps this recipient to signature and form fields in the document.\"\n        },\n        \"roles\": {\n          \"type\": \"array\",\n          \"description\": \"All role names assigned to this recipient.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"signing_order\": {\n          \"type\": [\"integer\", \"null\"],\n          \"minimum\": 1,\n          \"description\": \"Position in the sequential signing order. Null indicates no required order.\"\n  \
  \      },\n        \"has_completed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this recipient has completed all required signing actions.\"\n        },\n        \"contact_id\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Identifier of the linked contact record in the PandaDoc contacts directory.\"\n        },\n        \"shared_link\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Unique public URL for this recipient to access and sign the document.\"\n        }\n      }\n    },\n    \"TemplateReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the PandaDoc template used to generate a document.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the template.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display\
  \ name of the template.\"\n        }\n      }\n    },\n    \"MonetaryAmount\": {\n      \"type\": \"object\",\n      \"description\": \"A monetary value with associated currency.\",\n      \"required\": [\"amount\", \"currency\"],\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"string\",\n          \"description\": \"Numeric string representation of the monetary value.\",\n          \"pattern\": \"^-?[0-9]+(\\\\.[0-9]+)?$\",\n          \"example\": \"1250.00\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 three-letter currency code.\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"example\": \"USD\"\n        }\n      }\n    },\n    \"LinkedObject\": {\n      \"type\": \"object\",\n      \"description\": \"A link between a PandaDoc document and an external CRM or system entity.\",\n      \"properties\": {\n        \"provider\": {\n          \"type\": \"string\",\n          \"description\": \"Name\
  \ of the external system or CRM provider.\",\n          \"example\": \"salesforce\"\n        },\n        \"entity_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of entity in the external system.\",\n          \"example\": \"opportunity\"\n        },\n        \"entity_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the entity in the external system.\"\n        }\n      }\n    },\n    \"DocumentField\": {\n      \"type\": \"object\",\n      \"description\": \"A fillable or signable field within a PandaDoc document.\",\n      \"required\": [\"name\", \"type\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Field name as defined in the template or document.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Field type determining the kind of input or interaction required.\",\n          \"enum\": [\n        \
  \    \"signature\",\n            \"initials\",\n            \"text\",\n            \"date\",\n            \"checkbox\",\n            \"radio\",\n            \"select\",\n            \"attachment\",\n            \"payment\"\n          ]\n        },\n        \"value\": {\n          \"description\": \"Current value of the field. Type varies by field type.\"\n        },\n        \"role\": {\n          \"type\": \"string\",\n          \"description\": \"Recipient role name assigned to complete this field.\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this field must be filled before the document can be completed.\"\n        }\n      }\n    },\n    \"DocumentToken\": {\n      \"type\": \"object\",\n      \"description\": \"A content placeholder token in a document or template.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Token placeholder\
  \ name as defined in the template.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"Substitution value injected into the document at the token location.\"\n        }\n      }\n    },\n    \"PricingLineItem\": {\n      \"type\": \"object\",\n      \"description\": \"A single product or service line item in a document pricing table.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the line item within the pricing table.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the product or service.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the product or service.\"\n        },\n        \"qty\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity of the item.\",\n          \"minimum\": 0\n        },\n        \"\
  price\": {\n          \"type\": \"number\",\n          \"description\": \"Unit price of the item.\",\n          \"minimum\": 0\n        },\n        \"discount\": {\n          \"type\": \"object\",\n          \"description\": \"Discount applied to this line item.\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\"percent\", \"absolute\"],\n              \"description\": \"Whether the discount is a percentage or a fixed amount.\"\n            },\n            \"value\": {\n              \"type\": \"number\",\n              \"description\": \"Discount value.\",\n              \"minimum\": 0\n            }\n          }\n        },\n        \"tax_first\": {\n          \"type\": \"object\",\n          \"description\": \"First tax applied to the line item.\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\"percent\", \"absolute\"],\n              \"description\"\
  : \"Tax type.\"\n            },\n            \"value\": {\n              \"type\": \"number\",\n              \"description\": \"Tax value.\",\n              \"minimum\": 0\n            }\n          }\n        },\n        \"subtotal\": {\n          \"type\": \"number\",\n          \"description\": \"Calculated subtotal for this line item after discounts and before tax.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/json-schema/pandadoc-document-schema.json
tags:
- Document Automation
- E-Signature
- Document Management
- Document Generation
- Webhooks
title: PandaDoc Document
---
