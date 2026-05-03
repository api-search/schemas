---
description: Schema describing the JSON representation of a SAML 2.0 AuthnRequest message as defined in OASIS SAML 2.0 Core Section 3.4.1. An AuthnRequest is sent by a Service Provider to an Identity Provider to request authentication of a principal.
layout: schema
name: SAML 2.0 AuthnRequest
properties_list:
- description: A unique identifier for the request. The value MUST be generated using a mechanism that ensures uniqueness.
  name: ID
  type: string
- description: The SAML version of the request. MUST be '2.0'.
  name: Version
  type: string
- description: The time instant of issuance of the request in UTC.
  name: IssueInstant
  type: string
- description: The URI reference indicating the address to which the request has been sent.
  name: Destination
  type: string
- description: The entity that generated the request message. Typically the entityID of the Service Provider.
  name: Issuer
  type: string
- description: The URL to which the Identity Provider MUST return the SAML Response.
  name: AssertionConsumerServiceURL
  type: string
- description: An index referencing a particular AssertionConsumerService endpoint in the SP metadata.
  name: AssertionConsumerServiceIndex
  type: integer
- description: The SAML binding URI that the IdP should use to return the Response message.
  name: ProtocolBinding
  type: string
- description: If true, the Identity Provider MUST authenticate the presenter directly rather than rely on a previous security context.
  name: ForceAuthn
  type: boolean
- description: If true, the Identity Provider MUST NOT visibly take control of the user interface from the requester.
  name: IsPassive
  type: boolean
- description: Specifies constraints on the name identifier to be used to represent the requested subject.
  name: NameIDPolicy
  type: object
- description: Specifies the authentication context requirements for the authentication statement.
  name: RequestedAuthnContext
  type: object
- description: Indicates whether consent has been obtained from the principal for the request.
  name: Consent
  type: string
provider_name: SAML
provider_slug: saml
schema_file: json-schema/saml-authn-request.json
slug: saml-authn-request
source_filename: saml-authn-request.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"saml-authn-request.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SAML 2.0 AuthnRequest\",\n  \"description\": \"Schema describing the JSON representation of a SAML 2.0 AuthnRequest message as defined in OASIS SAML 2.0 Core Section 3.4.1. An AuthnRequest is sent by a Service Provider to an Identity Provider to request authentication of a principal.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ID\",\n    \"Version\",\n    \"IssueInstant\",\n    \"Issuer\"\n  ],\n  \"properties\": {\n    \"ID\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the request. The value MUST be generated using a mechanism that ensures uniqueness.\"\n    },\n    \"Version\": {\n      \"type\": \"string\",\n      \"description\": \"The SAML version of the request. MUST be '2.0'.\",\n      \"const\": \"2.0\"\n    },\n    \"IssueInstant\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"The time instant of issuance of the request in UTC.\"\n    },\n    \"Destination\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URI reference indicating the address to which the request has been sent.\"\n    },\n    \"Issuer\": {\n      \"type\": \"string\",\n      \"description\": \"The entity that generated the request message. Typically the entityID of the Service Provider.\"\n    },\n    \"AssertionConsumerServiceURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to which the Identity Provider MUST return the SAML Response.\"\n    },\n    \"AssertionConsumerServiceIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"An index referencing a particular AssertionConsumerService endpoint in the SP metadata.\",\n      \"minimum\": 0\n    },\n    \"ProtocolBinding\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The\
  \ SAML binding URI that the IdP should use to return the Response message.\",\n      \"examples\": [\n        \"urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\",\n        \"urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Artifact\"\n      ]\n    },\n    \"ForceAuthn\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the Identity Provider MUST authenticate the presenter directly rather than rely on a previous security context.\",\n      \"default\": false\n    },\n    \"IsPassive\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the Identity Provider MUST NOT visibly take control of the user interface from the requester.\",\n      \"default\": false\n    },\n    \"NameIDPolicy\": {\n      \"type\": \"object\",\n      \"description\": \"Specifies constraints on the name identifier to be used to represent the requested subject.\",\n      \"properties\": {\n        \"Format\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"\
  description\": \"The URI reference for the requested NameID format.\",\n          \"examples\": [\n            \"urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress\",\n            \"urn:oasis:names:tc:SAML:2.0:nameid-format:persistent\",\n            \"urn:oasis:names:tc:SAML:2.0:nameid-format:transient\",\n            \"urn:oasis:names:tc:SAML:1.1:nameid-format:unspecified\"\n          ]\n        },\n        \"AllowCreate\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the Identity Provider is allowed to create a new identifier to represent the principal.\",\n          \"default\": false\n        },\n        \"SPNameQualifier\": {\n          \"type\": \"string\",\n          \"description\": \"Further qualifies a name identifier with the name of a Service Provider or affiliation of providers.\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"RequestedAuthnContext\": {\n      \"type\": \"object\",\n      \"description\": \"Specifies\
  \ the authentication context requirements for the authentication statement.\",\n      \"properties\": {\n        \"Comparison\": {\n          \"type\": \"string\",\n          \"description\": \"How the requested context should be compared to the context used by the Identity Provider.\",\n          \"enum\": [\n            \"exact\",\n            \"minimum\",\n            \"maximum\",\n            \"better\"\n          ],\n          \"default\": \"exact\"\n        },\n        \"AuthnContextClassRef\": {\n          \"type\": \"array\",\n          \"description\": \"The authentication context class references that are acceptable.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"examples\": [\n            [\n              \"urn:oasis:names:tc:SAML:2.0:ac:classes:PasswordProtectedTransport\",\n              \"urn:oasis:names:tc:SAML:2.0:ac:classes:X509\"\n            ]\n          ]\n        }\n      },\n      \"additionalProperties\"\
  : true\n    },\n    \"Consent\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Indicates whether consent has been obtained from the principal for the request.\",\n      \"examples\": [\n        \"urn:oasis:names:tc:SAML:2.0:consent:unspecified\",\n        \"urn:oasis:names:tc:SAML:2.0:consent:obtained\"\n      ]\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/saml/refs/heads/main/json-schema/saml-authn-request.json
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
title: SAML 2.0 AuthnRequest
---
