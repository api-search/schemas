---
description: ''
layout: schema
name: APIDefinition
properties_list:
- description: ''
  name: active
  type: boolean
- description: ''
  name: allowed_ips
  type: array
- description: ''
  name: api_id
  type: string
- description: ''
  name: auth_configs
  type: object
- description: ''
  name: base_identity_provided_by
  type: string
- description: ''
  name: basic_auth
  type: object
- description: ''
  name: blacklisted_ips
  type: array
- description: ''
  name: certificate_pinning_disabled
  type: boolean
- description: ''
  name: certificates
  type: array
- description: ''
  name: client_certificates
  type: array
- description: ''
  name: config_data
  type: object
- description: ''
  name: config_data_disabled
  type: boolean
- description: ''
  name: custom_middleware_bundle
  type: string
- description: ''
  name: custom_middleware_bundle_disabled
  type: boolean
- description: ''
  name: custom_plugin_auth_enabled
  type: boolean
- description: ''
  name: detailed_tracing
  type: boolean
- description: ''
  name: disable_quota
  type: boolean
- description: ''
  name: disable_rate_limit
  type: boolean
- description: ''
  name: do_not_track
  type: boolean
- description: ''
  name: domain
  type: string
- description: ''
  name: domain_disabled
  type: boolean
- description: ''
  name: dont_set_quota_on_create
  type: boolean
- description: ''
  name: enable_batch_request_support
  type: boolean
- description: ''
  name: enable_context_vars
  type: boolean
- description: ''
  name: enable_coprocess_auth
  type: boolean
- description: ''
  name: enable_detailed_recording
  type: boolean
- description: ''
  name: enable_ip_blacklisting
  type: boolean
- description: ''
  name: enable_ip_whitelisting
  type: boolean
- description: ''
  name: enable_jwt
  type: boolean
- description: ''
  name: enable_proxy_protocol
  type: boolean
- description: ''
  name: enable_signature_checking
  type: boolean
- description: ''
  name: expiration
  type: string
- description: ''
  name: expire_analytics_after
  type: integer
- description: ''
  name: hmac_allowed_algorithms
  type: array
- description: ''
  name: hmac_allowed_clock_skew
  type: number
- description: ''
  name: id
  type: string
- description: ''
  name: idp_client_id_mapping_disabled
  type: boolean
- description: ''
  name: internal
  type: boolean
- description: ''
  name: is_oas
  type: boolean
- description: ''
  name: jwt_client_base_field
  type: string
- description: ''
  name: jwt_default_policies
  type: array
- description: ''
  name: jwt_expires_at_validation_skew
  type: integer
- description: ''
  name: jwt_identity_base_field
  type: string
- description: ''
  name: jwt_issued_at_validation_skew
  type: integer
- description: ''
  name: jwt_not_before_validation_skew
  type: integer
- description: ''
  name: jwt_policy_field_name
  type: string
- description: ''
  name: jwt_scope_claim_name
  type: string
- description: ''
  name: jwt_scope_to_policy_mapping
  type: object
- description: ''
  name: jwt_signing_method
  type: string
- description: ''
  name: jwt_skip_kid
  type: boolean
- description: ''
  name: jwt_source
  type: string
- description: ''
  name: listen_port
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: oauth_meta
  type: object
- description: ''
  name: org_id
  type: string
- description: ''
  name: pinned_public_keys
  type: object
- description: ''
  name: protocol
  type: string
- description: ''
  name: response_processors
  type: array
- description: ''
  name: session_lifetime
  type: integer
- description: ''
  name: session_lifetime_respects_key_expiration
  type: boolean
- description: ''
  name: slug
  type: string
- description: ''
  name: strip_auth_data
  type: boolean
- description: ''
  name: tag_headers
  type: array
- description: ''
  name: tags
  type: array
- description: ''
  name: tags_disabled
  type: boolean
- description: ''
  name: upstream_certificates
  type: object
- description: ''
  name: upstream_certificates_disabled
  type: boolean
- description: ''
  name: use_basic_auth
  type: boolean
- description: ''
  name: use_go_plugin_auth
  type: boolean
- description: ''
  name: use_keyless
  type: boolean
- description: ''
  name: use_mutual_tls_auth
  type: boolean
- description: ''
  name: use_oauth2
  type: boolean
- description: ''
  name: use_openid
  type: boolean
- description: ''
  name: use_standard_auth
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-api-definition-schema.json
slug: tyk-gateway-api-definition
source_filename: tyk-gateway-api-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"APIDefinition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"active\": {\n      \"type\": \"boolean\"\n    },\n    \"allowed_ips\": {\n      \"type\": \"array\"\n    },\n    \"api_id\": {\n      \"type\": \"string\"\n    },\n    \"auth_configs\": {\n      \"type\": \"object\"\n    },\n    \"base_identity_provided_by\": {\n      \"type\": \"string\"\n    },\n    \"basic_auth\": {\n      \"type\": \"object\"\n    },\n    \"blacklisted_ips\": {\n      \"type\": \"array\"\n    },\n    \"certificate_pinning_disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"certificates\": {\n      \"type\": \"array\"\n    },\n    \"client_certificates\": {\n      \"type\": \"array\"\n    },\n    \"config_data\": {\n      \"type\": \"object\"\n    },\n    \"config_data_disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"custom_middleware_bundle\": {\n      \"type\": \"string\"\n    },\n    \"\
  custom_middleware_bundle_disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"custom_plugin_auth_enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"detailed_tracing\": {\n      \"type\": \"boolean\"\n    },\n    \"disable_quota\": {\n      \"type\": \"boolean\"\n    },\n    \"disable_rate_limit\": {\n      \"type\": \"boolean\"\n    },\n    \"do_not_track\": {\n      \"type\": \"boolean\"\n    },\n    \"domain\": {\n      \"type\": \"string\"\n    },\n    \"domain_disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"dont_set_quota_on_create\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_batch_request_support\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_context_vars\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_coprocess_auth\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_detailed_recording\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_ip_blacklisting\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_ip_whitelisting\"\
  : {\n      \"type\": \"boolean\"\n    },\n    \"enable_jwt\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_proxy_protocol\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_signature_checking\": {\n      \"type\": \"boolean\"\n    },\n    \"expiration\": {\n      \"type\": \"string\"\n    },\n    \"expire_analytics_after\": {\n      \"type\": \"integer\"\n    },\n    \"hmac_allowed_algorithms\": {\n      \"type\": \"array\"\n    },\n    \"hmac_allowed_clock_skew\": {\n      \"type\": \"number\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"idp_client_id_mapping_disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"internal\": {\n      \"type\": \"boolean\"\n    },\n    \"is_oas\": {\n      \"type\": \"boolean\"\n    },\n    \"jwt_client_base_field\": {\n      \"type\": \"string\"\n    },\n    \"jwt_default_policies\": {\n      \"type\": \"array\"\n    },\n    \"jwt_expires_at_validation_skew\": {\n      \"type\": \"integer\"\n    },\n    \"jwt_identity_base_field\"\
  : {\n      \"type\": \"string\"\n    },\n    \"jwt_issued_at_validation_skew\": {\n      \"type\": \"integer\"\n    },\n    \"jwt_not_before_validation_skew\": {\n      \"type\": \"integer\"\n    },\n    \"jwt_policy_field_name\": {\n      \"type\": \"string\"\n    },\n    \"jwt_scope_claim_name\": {\n      \"type\": \"string\"\n    },\n    \"jwt_scope_to_policy_mapping\": {\n      \"type\": \"object\"\n    },\n    \"jwt_signing_method\": {\n      \"type\": \"string\"\n    },\n    \"jwt_skip_kid\": {\n      \"type\": \"boolean\"\n    },\n    \"jwt_source\": {\n      \"type\": \"string\"\n    },\n    \"listen_port\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"oauth_meta\": {\n      \"type\": \"object\"\n    },\n    \"org_id\": {\n      \"type\": \"string\"\n    },\n    \"pinned_public_keys\": {\n      \"type\": \"object\"\n    },\n    \"protocol\": {\n      \"type\": \"string\"\n    },\n    \"response_processors\": {\n      \"type\"\
  : \"array\"\n    },\n    \"session_lifetime\": {\n      \"type\": \"integer\"\n    },\n    \"session_lifetime_respects_key_expiration\": {\n      \"type\": \"boolean\"\n    },\n    \"slug\": {\n      \"type\": \"string\"\n    },\n    \"strip_auth_data\": {\n      \"type\": \"boolean\"\n    },\n    \"tag_headers\": {\n      \"type\": \"array\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"tags_disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"upstream_certificates\": {\n      \"type\": \"object\"\n    },\n    \"upstream_certificates_disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"use_basic_auth\": {\n      \"type\": \"boolean\"\n    },\n    \"use_go_plugin_auth\": {\n      \"type\": \"boolean\"\n    },\n    \"use_keyless\": {\n      \"type\": \"boolean\"\n    },\n    \"use_mutual_tls_auth\": {\n      \"type\": \"boolean\"\n    },\n    \"use_oauth2\": {\n      \"type\": \"boolean\"\n    },\n    \"use_openid\": {\n      \"type\": \"boolean\"\n    },\n\
  \    \"use_standard_auth\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-api-definition-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: APIDefinition
---
