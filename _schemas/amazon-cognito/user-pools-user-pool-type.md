---
description: A container for information about the user pool.
layout: schema
name: UserPoolType
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Name
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
  name: Status
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: SchemaAttributes
  type: object
- description: ''
  name: AutoVerifiedAttributes
  type: object
- description: ''
  name: AliasAttributes
  type: object
- description: ''
  name: UsernameAttributes
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
  name: EstimatedNumberOfUsers
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
  name: SmsConfigurationFailure
  type: object
- description: ''
  name: EmailConfigurationFailure
  type: object
- description: ''
  name: Domain
  type: object
- description: ''
  name: CustomDomain
  type: object
- description: ''
  name: AdminCreateUserConfig
  type: object
- description: ''
  name: UserPoolAddOns
  type: object
- description: ''
  name: UsernameConfiguration
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: AccountRecoverySetting
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-user-pool-type-schema.json
slug: user-pools-user-pool-type
source_filename: user-pools-user-pool-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-pool-type-schema.json\",\n  \"title\": \"UserPoolType\",\n  \"description\": \"A container for information about the user pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The ID of the user pool.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolNameType\"\n        },\n        {\n          \"description\": \"The name of the user pool.\"\n        }\n      ]\n    },\n    \"Policies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolPolicyType\"\n        },\n        {\n          \"description\": \"The policies associated\
  \ with the user pool.\"\n        }\n      ]\n    },\n    \"DeletionProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeletionProtectionType\"\n        },\n        {\n          \"description\": \"<p>When active, <code>DeletionProtection</code> prevents accidental deletion of your user pool. Before you can delete a user pool that you have protected against deletion, you must deactivate this feature.</p> <p>When you try to delete a protected user pool in a <code>DeleteUserPool</code> API request, Amazon Cognito returns an <code>InvalidParameterException</code> error. To delete a protected user pool, send a new <code>DeleteUserPool</code> request after you deactivate deletion protection in an <code>UpdateUserPool</code> API request.</p>\"\n        }\n      ]\n    },\n    \"LambdaConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaConfigType\"\n        },\n        {\n          \"description\": \"The Lambda triggers\
  \ associated with the user pool.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusType\"\n        },\n        {\n          \"description\": \"The status of a user pool.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was modified.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was created.\"\n        }\n      ]\n    },\n    \"SchemaAttributes\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/SchemaAttributesListType\"\n        },\n        {\n          \"description\": \"<p>A list of the user attributes and their properties in your user pool. The attribute schema contains standard attributes, custom attributes with a <code>custom:</code> prefix, and developer attributes with a <code>dev:</code> prefix. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-attributes.html\\\">User pool attributes</a>.</p> <p>Developer-only attributes are a legacy feature of user pools, are read-only to all app clients. You can create and update developer-only attributes only with IAM-authenticated API operations. Use app client read/write permissions instead.</p>\"\n        }\n      ]\n    },\n    \"AutoVerifiedAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VerifiedAttributesListType\"\n        },\n        {\n          \"description\"\
  : \"The attributes that are auto-verified in a user pool.\"\n        }\n      ]\n    },\n    \"AliasAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasAttributesListType\"\n        },\n        {\n          \"description\": \"The attributes that are aliased in a user pool.\"\n        }\n      ]\n    },\n    \"UsernameAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameAttributesListType\"\n        },\n        {\n          \"description\": \"Specifies whether a user can use an email address or phone number as a username when they sign up.\"\n        }\n      ]\n    },\n    \"SmsVerificationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsVerificationMessageType\"\n        },\n        {\n          \"description\": \"This parameter is no longer used. See <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_VerificationMessageTemplateType.html\\\
  \">VerificationMessageTemplateType</a>.\"\n        }\n      ]\n    },\n    \"EmailVerificationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationMessageType\"\n        },\n        {\n          \"description\": \"This parameter is no longer used. See <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_VerificationMessageTemplateType.html\\\">VerificationMessageTemplateType</a>.\"\n        }\n      ]\n    },\n    \"EmailVerificationSubject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationSubjectType\"\n        },\n        {\n          \"description\": \"This parameter is no longer used. See <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_VerificationMessageTemplateType.html\\\">VerificationMessageTemplateType</a>.\"\n        }\n      ]\n    },\n    \"VerificationMessageTemplate\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/VerificationMessageTemplateType\"\n        },\n        {\n          \"description\": \"The template for verification messages.\"\n        }\n      ]\n    },\n    \"SmsAuthenticationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsVerificationMessageType\"\n        },\n        {\n          \"description\": \"The contents of the SMS authentication message.\"\n        }\n      ]\n    },\n    \"UserAttributeUpdateSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserAttributeUpdateSettingsType\"\n        },\n        {\n          \"description\": \"The settings for updates to user attributes. These settings include the property <code>AttributesRequireVerificationBeforeUpdate</code>, a user-pool setting that tells Amazon Cognito how to handle changes to the value of your users' email address and phone number attributes. For more information, see <a href=\\\"\
  https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-email-phone-verification.html#user-pool-settings-verifications-verify-attribute-updates\\\"> Verifying updates to email addresses and phone numbers</a>.\"\n        }\n      ]\n    },\n    \"MfaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolMfaType\"\n        },\n        {\n          \"description\": \"<p>Can be one of the following values:</p> <ul> <li> <p> <code>OFF</code> - MFA tokens aren't required and can't be specified during user registration.</p> </li> <li> <p> <code>ON</code> - MFA tokens are required for all user registrations. You can only specify required when you're initially creating a user pool.</p> </li> <li> <p> <code>OPTIONAL</code> - Users have the option when registering to create an MFA token.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"DeviceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceConfigurationType\"\
  \n        },\n        {\n          \"description\": \"<p>The device-remembering configuration for a user pool. A null value indicates that you have deactivated device remembering in your user pool.</p> <note> <p>When you provide a value for any <code>DeviceConfiguration</code> field, you activate the Amazon Cognito device-remembering feature.</p> </note>\"\n        }\n      ]\n    },\n    \"EstimatedNumberOfUsers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerType\"\n        },\n        {\n          \"description\": \"A number estimating the size of the user pool.\"\n        }\n      ]\n    },\n    \"EmailConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailConfigurationType\"\n        },\n        {\n          \"description\": \"The email configuration of your user pool. The email configuration type sets your preferred sending method, Amazon Web Services Region, and sender for messages from your user\
  \ pool.\"\n        }\n      ]\n    },\n    \"SmsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsConfigurationType\"\n        },\n        {\n          \"description\": \"The SMS configuration with the settings that your Amazon Cognito user pool must use to send an SMS message from your Amazon Web Services account through Amazon Simple Notification Service. To send SMS messages with Amazon SNS in the Amazon Web Services Region that you want, the Amazon Cognito user pool uses an Identity and Access Management (IAM) role in your Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"UserPoolTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolTagsType\"\n        },\n        {\n          \"description\": \"The tags that are assigned to the user pool. A tag is a label that you can apply to user pools to categorize and manage them in different ways, such as by purpose, owner, environment, or other\
  \ criteria.\"\n        }\n      ]\n    },\n    \"SmsConfigurationFailure\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"<p>The reason why the SMS configuration can't send the messages to your users.</p> <p>This message might include comma-separated values to describe why your SMS configuration can't send messages to user pool end users.</p> <dl> <dt>InvalidSmsRoleAccessPolicyException</dt> <dd> <p>The Identity and Access Management role that Amazon Cognito uses to send SMS messages isn't properly configured. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_SmsConfigurationType.html\\\">SmsConfigurationType</a>.</p> </dd> <dt>SNSSandbox</dt> <dd> <p>The Amazon Web Services account is in the SNS SMS Sandbox and messages will only reach verified end users. This parameter won\\u2019t get populated with SNSSandbox if the user\
  \ creating the user pool doesn\\u2019t have SNS permissions. To learn how to move your Amazon Web Services account out of the sandbox, see <a href=\\\"https://docs.aws.amazon.com/sns/latest/dg/sns-sms-sandbox-moving-to-production.html\\\">Moving out of the SMS sandbox</a>.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"EmailConfigurationFailure\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"Deprecated. Review error codes from API requests with <code>EventSource:cognito-idp.amazonaws.com</code> in CloudTrail for information about problems with user pool email configuration.\"\n        }\n      ]\n    },\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainType\"\n        },\n        {\n          \"description\": \"The domain prefix, if the user pool has a domain associated with it.\"\n        }\n      ]\n    },\n    \"CustomDomain\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainType\"\n        },\n        {\n          \"description\": \"<p>A custom domain name that you provide to Amazon Cognito. This parameter applies only if you use a custom domain to host the sign-up and sign-in pages for your application. An example of a custom domain name might be <code>auth.example.com</code>.</p> <p>For more information about adding a custom domain to your user pool, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-add-custom-domain.html\\\">Using Your Own Domain for the Hosted UI</a>.</p>\"\n        }\n      ]\n    },\n    \"AdminCreateUserConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdminCreateUserConfigType\"\n        },\n        {\n          \"description\": \"The configuration for <code>AdminCreateUser</code> requests.\"\n        }\n      ]\n    },\n    \"UserPoolAddOns\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/UserPoolAddOnsType\"\n        },\n        {\n          \"description\": \"<p>User pool add-ons. Contains settings for activation of advanced security features. To log user security information but take no action, set to <code>AUDIT</code>. To configure automatic security responses to risky traffic to your user pool, set to <code>ENFORCED</code>.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pool-settings-advanced-security.html\\\">Adding advanced security to a user pool</a>.</p>\"\n        }\n      ]\n    },\n    \"UsernameConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameConfigurationType\"\n        },\n        {\n          \"description\": \"Case sensitivity of the username input for the selected sign-in option. For example, when case sensitivity is set to <code>False</code>, users can sign in using either \\\"username\\\
  \" or \\\"Username\\\". This configuration is immutable once it has been set. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_UsernameConfigurationType.html\\\">UsernameConfigurationType</a>.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the user pool.\"\n        }\n      ]\n    },\n    \"AccountRecoverySetting\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountRecoverySettingType\"\n        },\n        {\n          \"description\": \"The available verified method a user can use to recover their password when they call <code>ForgotPassword</code>. You can use this setting to define a preferred method when a user has more than one method available. With this setting, SMS doesn't qualify for a valid password recovery\
  \ mechanism if the user also has SMS multi-factor authentication (MFA) activated. In the absence of this setting, Amazon Cognito uses the legacy behavior to determine the recovery method where SMS is preferred through email.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-pool-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UserPoolType
---
