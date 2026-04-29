---
description: Represents the request to update the user pool.
layout: schema
name: UpdateUserPoolRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Policies
  type: object
- description: ''
  name: DeletionProtection
  type: object
- description: ''
  name: LambdaConfig
  type: object
- description: ''
  name: AutoVerifiedAttributes
  type: object
- description: ''
  name: SmsVerificationMessage
  type: object
- description: ''
  name: EmailVerificationMessage
  type: object
- description: ''
  name: EmailVerificationSubject
  type: object
- description: ''
  name: VerificationMessageTemplate
  type: object
- description: ''
  name: SmsAuthenticationMessage
  type: object
- description: ''
  name: UserAttributeUpdateSettings
  type: object
- description: ''
  name: MfaConfiguration
  type: object
- description: ''
  name: DeviceConfiguration
  type: object
- description: ''
  name: EmailConfiguration
  type: object
- description: ''
  name: SmsConfiguration
  type: object
- description: ''
  name: UserPoolTags
  type: object
- description: ''
  name: AdminCreateUserConfig
  type: object
- description: ''
  name: UserPoolAddOns
  type: object
- description: ''
  name: AccountRecoverySetting
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-update-user-pool-request-schema.json
slug: user-pools-update-user-pool-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-user-pool-request-schema.json\",\n  \"title\": \"UpdateUserPoolRequest\",\n  \"description\": \"Represents the request to update the user pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool you want to update.\"\n        }\n      ]\n    },\n    \"Policies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolPolicyType\"\n        },\n        {\n          \"description\": \"A container with the policies you want to update in a user pool.\"\n        }\n      ]\n    },\n    \"DeletionProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/DeletionProtectionType\"\n        },\n        {\n          \"description\": \"<p>When active, <code>DeletionProtection</code> prevents accidental deletion of your user pool. Before you can delete a user pool that you have protected against deletion, you must deactivate this feature.</p> <p>When you try to delete a protected user pool in a <code>DeleteUserPool</code> API request, Amazon Cognito returns an <code>InvalidParameterException</code> error. To delete a protected user pool, send a new <code>DeleteUserPool</code> request after you deactivate deletion protection in an <code>UpdateUserPool</code> API request.</p>\"\n        }\n      ]\n    },\n    \"LambdaConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaConfigType\"\n        },\n        {\n          \"description\": \"The Lambda configuration information from the request to update the user pool.\"\n        }\n      ]\n    },\n    \"AutoVerifiedAttributes\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VerifiedAttributesListType\"\n        },\n        {\n          \"description\": \"The attributes that are automatically verified when Amazon Cognito requests to update user pools.\"\n        }\n      ]\n    },\n    \"SmsVerificationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsVerificationMessageType\"\n        },\n        {\n          \"description\": \"This parameter is no longer used. See <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_VerificationMessageTemplateType.html\\\">VerificationMessageTemplateType</a>.\"\n        }\n      ]\n    },\n    \"EmailVerificationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationMessageType\"\n        },\n        {\n          \"description\": \"This parameter is no longer used. See <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_VerificationMessageTemplateType.html\\\
  \">VerificationMessageTemplateType</a>.\"\n        }\n      ]\n    },\n    \"EmailVerificationSubject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationSubjectType\"\n        },\n        {\n          \"description\": \"This parameter is no longer used. See <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_VerificationMessageTemplateType.html\\\">VerificationMessageTemplateType</a>.\"\n        }\n      ]\n    },\n    \"VerificationMessageTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VerificationMessageTemplateType\"\n        },\n        {\n          \"description\": \"The template for verification messages.\"\n        }\n      ]\n    },\n    \"SmsAuthenticationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsVerificationMessageType\"\n        },\n        {\n          \"description\": \"The contents of the SMS authentication\
  \ message.\"\n        }\n      ]\n    },\n    \"UserAttributeUpdateSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserAttributeUpdateSettingsType\"\n        },\n        {\n          \"description\": \"The settings for updates to user attributes. These settings include the property <code>AttributesRequireVerificationBeforeUpdate</code>, a user-pool setting that tells Amazon Cognito how to handle changes to the value of your users' email address and phone number attributes. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-email-phone-verification.html#user-pool-settings-verifications-verify-attribute-updates\\\"> Verifying updates to email addresses and phone numbers</a>.\"\n        }\n      ]\n    },\n    \"MfaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolMfaType\"\n        },\n        {\n          \"description\": \"<p>Possible\
  \ values include:</p> <ul> <li> <p> <code>OFF</code> - MFA tokens aren't required and can't be specified during user registration.</p> </li> <li> <p> <code>ON</code> - MFA tokens are required for all user registrations. You can only specify ON when you're initially creating a user pool. You can use the <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_SetUserPoolMfaConfig.html\\\">SetUserPoolMfaConfig</a> API operation to turn MFA \\\"ON\\\" for existing user pools. </p> </li> <li> <p> <code>OPTIONAL</code> - Users have the option when registering to create an MFA token.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"DeviceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceConfigurationType\"\n        },\n        {\n          \"description\": \"<p>The device-remembering configuration for a user pool. A null value indicates that you have deactivated device remembering in your user pool.</p>\
  \ <note> <p>When you provide a value for any <code>DeviceConfiguration</code> field, you activate the Amazon Cognito device-remembering feature.</p> </note>\"\n        }\n      ]\n    },\n    \"EmailConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailConfigurationType\"\n        },\n        {\n          \"description\": \"The email configuration of your user pool. The email configuration type sets your preferred sending method, Amazon Web Services Region, and sender for email invitation and verification messages from your user pool.\"\n        }\n      ]\n    },\n    \"SmsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsConfigurationType\"\n        },\n        {\n          \"description\": \"The SMS configuration with the settings that your Amazon Cognito user pool must use to send an SMS message from your Amazon Web Services account through Amazon Simple Notification Service. To send SMS messages\
  \ with Amazon SNS in the Amazon Web Services Region that you want, the Amazon Cognito user pool uses an Identity and Access Management (IAM) role in your Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"UserPoolTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolTagsType\"\n        },\n        {\n          \"description\": \"The tag keys and values to assign to the user pool. A tag is a label that you can use to categorize and manage user pools in different ways, such as by purpose, owner, environment, or other criteria.\"\n        }\n      ]\n    },\n    \"AdminCreateUserConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdminCreateUserConfigType\"\n        },\n        {\n          \"description\": \"The configuration for <code>AdminCreateUser</code> requests.\"\n        }\n      ]\n    },\n    \"UserPoolAddOns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolAddOnsType\"\
  \n        },\n        {\n          \"description\": \"<p>User pool add-ons. Contains settings for activation of advanced security features. To log user security information but take no action, set to <code>AUDIT</code>. To configure automatic security responses to risky traffic to your user pool, set to <code>ENFORCED</code>.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pool-settings-advanced-security.html\\\">Adding advanced security to a user pool</a>.</p>\"\n        }\n      ]\n    },\n    \"AccountRecoverySetting\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountRecoverySettingType\"\n        },\n        {\n          \"description\": \"The available verified method a user can use to recover their password when they call <code>ForgotPassword</code>. You can use this setting to define a preferred method when a user has more than one method available. With this setting, SMS doesn't\
  \ qualify for a valid password recovery mechanism if the user also has SMS multi-factor authentication (MFA) activated. In the absence of this setting, Amazon Cognito uses the legacy behavior to determine the recovery method where SMS is preferred through email.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-user-pool-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UpdateUserPoolRequest
---
