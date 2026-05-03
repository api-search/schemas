---
description: Schema describing the JSON representation of a SAML 2.0 Assertion as defined in OASIS SAML 2.0 Core Section 2. An assertion is a package of information that supplies one or more statements made by a SAML authority (typically an Identity Provider).
layout: schema
name: SAML 2.0 Assertion
properties_list:
- description: The SAML version of the assertion. MUST be '2.0'.
  name: Version
  type: string
- description: A unique identifier for the assertion.
  name: ID
  type: string
- description: The time instant of issuance in UTC.
  name: IssueInstant
  type: string
- description: The SAML authority that created and is responsible for the assertion. Typically the entityID of the Identity Provider.
  name: Issuer
  type: string
- description: The principal that is the subject of the statements in the assertion.
  name: Subject
  type: object
- description: Conditions that MUST be evaluated when assessing the validity of the assertion.
  name: Conditions
  type: object
- description: Statements about the authentication event.
  name: AuthnStatement
  type: array
- description: Statements containing attributes about the subject.
  name: AttributeStatement
  type: array
provider_name: SAML
provider_slug: saml
schema_file: json-schema/saml-assertion.json
slug: saml-assertion
source_filename: saml-assertion.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"saml-assertion.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SAML 2.0 Assertion\",\n  \"description\": \"Schema describing the JSON representation of a SAML 2.0 Assertion as defined in OASIS SAML 2.0 Core Section 2. An assertion is a package of information that supplies one or more statements made by a SAML authority (typically an Identity Provider).\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Version\",\n    \"ID\",\n    \"IssueInstant\",\n    \"Issuer\"\n  ],\n  \"properties\": {\n    \"Version\": {\n      \"type\": \"string\",\n      \"description\": \"The SAML version of the assertion. MUST be '2.0'.\",\n      \"const\": \"2.0\"\n    },\n    \"ID\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the assertion.\"\n    },\n    \"IssueInstant\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time instant of issuance in UTC.\"\
  \n    },\n    \"Issuer\": {\n      \"type\": \"string\",\n      \"description\": \"The SAML authority that created and is responsible for the assertion. Typically the entityID of the Identity Provider.\"\n    },\n    \"Subject\": {\n      \"type\": \"object\",\n      \"description\": \"The principal that is the subject of the statements in the assertion.\",\n      \"properties\": {\n        \"NameID\": {\n          \"type\": \"object\",\n          \"description\": \"The name identifier for the subject.\",\n          \"properties\": {\n            \"Format\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The format of the name identifier.\"\n            },\n            \"SPNameQualifier\": {\n              \"type\": \"string\",\n              \"description\": \"The Service Provider or affiliation that the identifier is scoped to.\"\n            },\n            \"value\": {\n              \"type\": \"string\",\n             \
  \ \"description\": \"The actual name identifier value.\"\n            }\n          }\n        },\n        \"SubjectConfirmation\": {\n          \"type\": \"array\",\n          \"description\": \"Information allowing the subject to be confirmed.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Method\": {\n                \"type\": \"string\",\n                \"format\": \"uri\",\n                \"description\": \"The confirmation method URI.\",\n                \"examples\": [\n                  \"urn:oasis:names:tc:SAML:2.0:cm:bearer\"\n                ]\n              },\n              \"SubjectConfirmationData\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"InResponseTo\": {\n                    \"type\": \"string\",\n                    \"description\": \"The ID of the AuthnRequest this assertion is in response to.\"\n                  },\n                  \"Recipient\"\
  : {\n                    \"type\": \"string\",\n                    \"format\": \"uri\",\n                    \"description\": \"The URI of the entity to which the assertion is addressed.\"\n                  },\n                  \"NotOnOrAfter\": {\n                    \"type\": \"string\",\n                    \"format\": \"date-time\",\n                    \"description\": \"The time instant after which the subject can no longer be confirmed.\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"Conditions\": {\n      \"type\": \"object\",\n      \"description\": \"Conditions that MUST be evaluated when assessing the validity of the assertion.\",\n      \"properties\": {\n        \"NotBefore\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The assertion MUST NOT be used before this time instant.\"\n        },\n        \"\
  NotOnOrAfter\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The assertion MUST NOT be used on or after this time instant.\"\n        },\n        \"AudienceRestriction\": {\n          \"type\": \"array\",\n          \"description\": \"The set of audiences that the assertion is intended for.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Audience\": {\n                \"type\": \"array\",\n                \"description\": \"URIs identifying intended audiences.\",\n                \"items\": {\n                  \"type\": \"string\",\n                  \"format\": \"uri\"\n                }\n              }\n            }\n          }\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"AuthnStatement\": {\n      \"type\": \"array\",\n      \"description\": \"Statements about the authentication event.\",\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"required\": [\n          \"AuthnInstant\",\n          \"AuthnContext\"\n        ],\n        \"properties\": {\n          \"AuthnInstant\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The time at which the authentication took place.\"\n          },\n          \"SessionIndex\": {\n            \"type\": \"string\",\n            \"description\": \"The index of the session at the Identity Provider.\"\n          },\n          \"SessionNotOnOrAfter\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The time at which the session expires.\"\n          },\n          \"AuthnContext\": {\n            \"type\": \"object\",\n            \"description\": \"The context of the authentication event.\",\n            \"properties\": {\n              \"AuthnContextClassRef\": {\n                \"type\": \"string\",\n                \"format\": \"uri\",\n              \
  \  \"description\": \"A URI reference identifying the authentication context class.\",\n                \"examples\": [\n                  \"urn:oasis:names:tc:SAML:2.0:ac:classes:PasswordProtectedTransport\"\n                ]\n              }\n            }\n          }\n        }\n      }\n    },\n    \"AttributeStatement\": {\n      \"type\": \"array\",\n      \"description\": \"Statements containing attributes about the subject.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Attribute\": {\n            \"type\": \"array\",\n            \"description\": \"The attributes associated with the subject.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"required\": [\n                \"Name\"\n              ],\n              \"properties\": {\n                \"Name\": {\n                  \"type\": \"string\",\n                  \"description\": \"The name of the attribute.\"\n                },\n          \
  \      \"NameFormat\": {\n                  \"type\": \"string\",\n                  \"format\": \"uri\",\n                  \"description\": \"The format of the attribute name.\",\n                  \"examples\": [\n                    \"urn:oasis:names:tc:SAML:2.0:attrname-format:uri\",\n                    \"urn:oasis:names:tc:SAML:2.0:attrname-format:basic\"\n                  ]\n                },\n                \"AttributeValue\": {\n                  \"type\": \"array\",\n                  \"description\": \"The values of the attribute.\",\n                  \"items\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/saml/refs/heads/main/json-schema/saml-assertion.json
tags:
- Authentication
- Authorization
- Federation
- Identity Management
- Open Standard
- Security
- Single Sign-On
- SSO
- XML
title: SAML 2.0 Assertion
---
