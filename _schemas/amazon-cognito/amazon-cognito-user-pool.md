---
description: Schema representing an Amazon Cognito user pool configuration and its properties.
layout: schema
name: Amazon Cognito User Pool
properties_list:
- description: The unique identifier for the user pool.
  name: Id
  type: string
- description: The name of the user pool.
  name: Name
  type: string
- description: The status of the user pool.
  name: Status
  type: string
- description: The Amazon Resource Name (ARN) for the user pool.
  name: Arn
  type: string
- description: The date and time when the user pool was created.
  name: CreationDate
  type: string
- description: The date and time when the user pool was last modified.
  name: LastModifiedDate
  type: string
- description: A number estimating the size of the user pool.
  name: EstimatedNumberOfUsers
  type: integer
- description: The multi-factor authentication (MFA) configuration.
  name: MfaConfiguration
  type: string
- description: The policies associated with the user pool.
  name: Policies
  type: object
- description: The attributes that are automatically verified.
  name: AutoVerifiedAttributes
  type: array
- description: Specifies whether email addresses or phone numbers can be used as user names when a user signs up.
  name: UsernameAttributes
  type: array
- description: The schema attributes for the user pool.
  name: SchemaAttributes
  type: array
- description: The email configuration for the user pool.
  name: EmailConfiguration
  type: object
- description: The SMS configuration for the user pool.
  name: SmsConfiguration
  type: object
- description: The tags that are assigned to the user pool.
  name: UserPoolTags
  type: object
- description: The configuration for AdminCreateUser requests.
  name: AdminCreateUserConfig
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/amazon-cognito-user-pool-schema.json
slug: amazon-cognito-user-pool
source_filename: amazon-cognito-user-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://amazon-cognito.apis.io/json-schema/amazon-cognito-user-pool-schema.json\",\n  \"title\": \"Amazon Cognito User Pool\",\n  \"description\": \"Schema representing an Amazon Cognito user pool configuration and its properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the user pool.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the user pool.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the user pool.\",\n      \"enum\": [\"Enabled\", \"Disabled\"]\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the user pool.\",\n      \"pattern\": \"^arn:aws:cognito-idp:[a-z0-9-]+:[0-9]+:userpool/[a-zA-Z0-9_-]+$\"\n    },\n    \"CreationDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the user pool was created.\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the user pool was last modified.\"\n    },\n    \"EstimatedNumberOfUsers\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"A number estimating the size of the user pool.\"\n    },\n    \"MfaConfiguration\": {\n      \"type\": \"string\",\n      \"enum\": [\"OFF\", \"ON\", \"OPTIONAL\"],\n      \"description\": \"The multi-factor authentication (MFA) configuration.\"\n    },\n    \"Policies\": {\n      \"type\": \"object\",\n      \"description\": \"The policies associated with the user pool.\",\n      \"properties\": {\n        \"PasswordPolicy\": {\n          \"type\": \"object\",\n          \"description\": \"The password policy for the user pool.\",\n         \
  \ \"properties\": {\n            \"MinimumLength\": {\n              \"type\": \"integer\",\n              \"minimum\": 6,\n              \"maximum\": 99,\n              \"description\": \"The minimum length of the password.\"\n            },\n            \"RequireUppercase\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether the password must contain at least one uppercase letter.\"\n            },\n            \"RequireLowercase\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether the password must contain at least one lowercase letter.\"\n            },\n            \"RequireNumbers\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether the password must contain at least one number.\"\n            },\n            \"RequireSymbols\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether the password must contain at least one symbol.\"\n            },\n           \
  \ \"TemporaryPasswordValidityDays\": {\n              \"type\": \"integer\",\n              \"minimum\": 0,\n              \"maximum\": 365,\n              \"description\": \"The number of days a temporary password is valid.\"\n            }\n          }\n        }\n      }\n    },\n    \"AutoVerifiedAttributes\": {\n      \"type\": \"array\",\n      \"description\": \"The attributes that are automatically verified.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"phone_number\", \"email\"]\n      }\n    },\n    \"UsernameAttributes\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies whether email addresses or phone numbers can be used as user names when a user signs up.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"phone_number\", \"email\"]\n      }\n    },\n    \"SchemaAttributes\": {\n      \"type\": \"array\",\n      \"description\": \"The schema attributes for the user pool.\",\n      \"items\": {\n       \
  \ \"type\": \"object\",\n        \"properties\": {\n          \"Name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the attribute.\"\n          },\n          \"AttributeDataType\": {\n            \"type\": \"string\",\n            \"enum\": [\"String\", \"Number\", \"DateTime\", \"Boolean\"],\n            \"description\": \"The data type of the attribute.\"\n          },\n          \"Mutable\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the attribute can be changed after creation.\"\n          },\n          \"Required\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the attribute is required during user registration.\"\n          },\n          \"StringAttributeConstraints\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"MinLength\": {\n                \"type\": \"string\",\n                \"description\": \"The minimum length.\"\n             \
  \ },\n              \"MaxLength\": {\n                \"type\": \"string\",\n                \"description\": \"The maximum length.\"\n              }\n            }\n          },\n          \"NumberAttributeConstraints\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"MinValue\": {\n                \"type\": \"string\",\n                \"description\": \"The minimum value.\"\n              },\n              \"MaxValue\": {\n                \"type\": \"string\",\n                \"description\": \"The maximum value.\"\n              }\n            }\n          }\n        },\n        \"required\": [\"Name\"]\n      }\n    },\n    \"EmailConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"The email configuration for the user pool.\",\n      \"properties\": {\n        \"SourceArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of a verified email address in Amazon SES.\"\n        },\n        \"ReplyToEmailAddress\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The destination to which the receiver of the email should reply.\"\n        },\n        \"EmailSendingAccount\": {\n          \"type\": \"string\",\n          \"enum\": [\"COGNITO_DEFAULT\", \"DEVELOPER\"],\n          \"description\": \"Specifies whether Amazon Cognito emails your users by using its built-in email functionality or your Amazon SES email configuration.\"\n        }\n      }\n    },\n    \"SmsConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"The SMS configuration for the user pool.\",\n      \"properties\": {\n        \"SnsCallerArn\": {\n          \"type\": \"string\",\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon SNS caller.\"\n        },\n        \"ExternalId\": {\n          \"type\": \"string\",\n          \"description\": \"The external ID.\"\n        },\n        \"SnsRegion\": {\n          \"type\": \"string\",\n \
  \         \"description\": \"The AWS Region to use with Amazon SNS integration.\"\n        }\n      },\n      \"required\": [\"SnsCallerArn\"]\n    },\n    \"UserPoolTags\": {\n      \"type\": \"object\",\n      \"description\": \"The tags that are assigned to the user pool.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"AdminCreateUserConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The configuration for AdminCreateUser requests.\",\n      \"properties\": {\n        \"AllowAdminCreateUserOnly\": {\n          \"type\": \"boolean\",\n          \"description\": \"Set to true if only the administrator is allowed to create user profiles.\"\n        },\n        \"UnusedAccountValidityDays\": {\n          \"type\": \"integer\",\n          \"description\": \"The user account expiration limit, in days, after which the account is no longer usable.\"\n        },\n        \"InviteMessageTemplate\": {\n          \"type\": \"object\",\n\
  \          \"properties\": {\n            \"SMSMessage\": {\n              \"type\": \"string\"\n            },\n            \"EmailMessage\": {\n              \"type\": \"string\"\n            },\n            \"EmailSubject\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"Name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/amazon-cognito-user-pool-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: Amazon Cognito User Pool
---
