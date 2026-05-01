---
description: Optional. The metadata of the LDAP server used to authenticate and authorize connections to the broker.
layout: schema
name: LdapServerMetadataOutput
properties_list:
- description: ''
  name: Hosts
  type: object
- description: ''
  name: RoleBase
  type: object
- description: ''
  name: RoleName
  type: object
- description: ''
  name: RoleSearchMatching
  type: object
- description: ''
  name: RoleSearchSubtree
  type: object
- description: ''
  name: ServiceAccountUsername
  type: object
- description: ''
  name: UserBase
  type: object
- description: ''
  name: UserRoleName
  type: object
- description: ''
  name: UserSearchMatching
  type: object
- description: ''
  name: UserSearchSubtree
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-ldap-server-metadata-output-schema.json
slug: mq-api-ldap-server-metadata-output
source_filename: mq-api-ldap-server-metadata-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-ldap-server-metadata-output-schema.json\",\n  \"title\": \"LdapServerMetadataOutput\",\n  \"description\": \"Optional. The metadata of the LDAP server used to authenticate and authorize connections to the broker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Hosts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hosts\"\n          },\n          \"description\": \"Specifies the location of the LDAP server such as AWS Directory Service for Microsoft Active Directory . Optional failover server.\"\n        }\n      ]\n    },\n    \"RoleBase\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n \
  \           \"name\": \"roleBase\"\n          },\n          \"description\": \"The distinguished name of the node in the directory information tree (DIT) to search for roles or groups. For example, ou=group, ou=corp, dc=corp,\\n                  dc=example, dc=com.\"\n        }\n      ]\n    },\n    \"RoleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleName\"\n          },\n          \"description\": \"Specifies the LDAP attribute that identifies the group name attribute in the object returned from the group membership query.\"\n        }\n      ]\n    },\n    \"RoleSearchMatching\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleSearchMatching\"\n          },\n          \"description\": \"The LDAP search filter used to find roles within the roleBase. The\
  \ distinguished name of the user matched by userSearchMatching is substituted into the {0} placeholder in the search filter. The client's username is substituted into the {1} placeholder. For example, if you set this option to (member=uid={1})for the user janedoe, the search filter becomes (member=uid=janedoe) after string substitution. It matches all role entries that have a member attribute equal to uid=janedoe under the subtree selected by the roleBase.\"\n        }\n      ]\n    },\n    \"RoleSearchSubtree\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleSearchSubtree\"\n          },\n          \"description\": \"The directory search scope for the role. If set to true, scope is to search the entire subtree.\"\n        }\n      ]\n    },\n    \"ServiceAccountUsername\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"serviceAccountUsername\"\n          },\n          \"description\": \"Service account username. A service account is an account in your LDAP server that has access to initiate a connection. For example, cn=admin,dc=corp, dc=example,\\n                  dc=com.\"\n        }\n      ]\n    },\n    \"UserBase\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userBase\"\n          },\n          \"description\": \"Select a particular subtree of the directory information tree (DIT) to search for user entries. The subtree is specified by a DN, which specifies the base node of the subtree. For example, by setting this option to ou=Users,ou=corp, dc=corp,\\n                  dc=example, dc=com, the search for user entries is restricted to the subtree beneath ou=Users, ou=corp, dc=corp, dc=example, dc=com.\"\n        }\n      ]\n \
  \   },\n    \"UserRoleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userRoleName\"\n          },\n          \"description\": \"Specifies the name of the LDAP attribute for the user group membership.\"\n        }\n      ]\n    },\n    \"UserSearchMatching\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userSearchMatching\"\n          },\n          \"description\": \"The LDAP search filter used to find users within the userBase. The client's username is substituted into the {0} placeholder in the search filter. For example, if this option is set to (uid={0}) and the received username is janedoe, the search filter becomes (uid=janedoe) after string substitution. It will result in matching an entry like uid=janedoe, ou=Users,ou=corp, dc=corp, dc=example,\\n   \
  \            dc=com.\"\n        }\n      ]\n    },\n    \"UserSearchSubtree\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userSearchSubtree\"\n          },\n          \"description\": \"The directory search scope for the user. If set to true, scope is to search the entire subtree.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Hosts\",\n    \"UserSearchMatching\",\n    \"UserBase\",\n    \"RoleSearchMatching\",\n    \"ServiceAccountUsername\",\n    \"RoleBase\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-ldap-server-metadata-output-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: LdapServerMetadataOutput
---
