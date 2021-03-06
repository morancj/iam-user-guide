# Actions, Resources, and Condition Keys for Amazon Pinpoint SMS and Voice Service<a name="list_amazonpinpointsmsandvoiceservice"></a>

Amazon Pinpoint SMS and Voice Service \(service prefix: `sms-voice`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/pinpoint/latest/developerguide/)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/pinpoint-sms-voice/latest/apireference/)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/pinpoint/latest/developerguide/permissions-actions.html#permissions-actions-apiactions) permission policies\.

**Topics**
+ [Actions Defined by Amazon Pinpoint SMS and Voice Service](#amazonpinpointsmsandvoiceservice-actions-as-permissions)
+ [Resources Defined by Amazon Pinpoint SMS and Voice Service](#amazonpinpointsmsandvoiceservice-resources-for-iam-policies)
+ [Condition Keys for Amazon Pinpoint SMS and Voice Service](#amazonpinpointsmsandvoiceservice-policy-keys)

## Actions Defined by Amazon Pinpoint SMS and Voice Service<a name="amazonpinpointsmsandvoiceservice-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access Level | Resource Types \(\*required\) | Condition Keys | Dependent Actions | 
| --- | --- | --- | --- | --- | --- | 
|   [ CreateConfigurationSet ](https://docs.aws.amazon.com/pinpoint-sms-voice/latest/apireference/v1-sms-voice-configuration-sets.html)  | Create a new configuration set\. After you create the configuration set, you can add one or more event destinations to it\. | Write |  |  |  | 
|   [ CreateConfigurationSetEventDestination ](https://docs.aws.amazon.com/pinpoint-sms-voice/latest/apireference/v1-sms-voice-configuration-sets-configurationsetname-event-destinations.html)  | Create a new event destination in a configuration set\. | Write |  |  |   iam:PassRole   | 
|   [ DeleteConfigurationSet ](https://docs.aws.amazon.com/pinpoint-sms-voice/latest/apireference/v1-sms-voice-configuration-sets-configurationsetname.html)  | Deletes an existing configuration set\. | Write |  |  |  | 
|   [ DeleteConfigurationSetEventDestination ](https://docs.aws.amazon.com/pinpoint-sms-voice/latest/apireference/v1-sms-voice-configuration-sets-configurationsetname-event-destinations-eventdestinationname.html)  | Deletes an event destination in a configuration set\. | Write |  |  |  | 
|   [ GetConfigurationSetEventDestinations ](https://docs.aws.amazon.com/pinpoint-sms-voice/latest/apireference/v1-sms-voice-configuration-sets-configurationsetname-event-destinations.html)  | Obtain information about an event destination, including the types of events it reports, the Amazon Resource Name \(ARN\) of the destination, and the name of the event destination\. | Read |  |  |  | 
|   [ ListConfigurationSets ](https://docs.aws.amazon.com/pinpoint-sms-voice/latest/apireference/v1-sms-voice-configuration-sets.html)  | Return a list of configuration sets\. This operation only returns the configuration sets that are associated with your account in the current AWS Region\. | Read |  |  |  | 
|   [ SendVoiceMessage ](https://docs.aws.amazon.com/pinpoint-sms-voice/latest/apireference/v1-sms-voice-voice-message.html)  | Create a new voice message and send it to a recipient's phone number\. | Write |  |  |  | 
|   [ UpdateConfigurationSetEventDestination ](https://docs.aws.amazon.com/pinpoint-sms-voice/latest/apireference/v1-sms-voice-configuration-sets-configurationsetname-event-destinations-eventdestinationname.html)  | Update an event destination in a configuration set\. An event destination is a location that you publish information about your voice calls to\. For example, you can log an event to an Amazon CloudWatch destination when a call fails\. | Write |  |  |   iam:PassRole   | 

## Resources Defined by Amazon Pinpoint SMS and Voice Service<a name="amazonpinpointsmsandvoiceservice-resources-for-iam-policies"></a>

Amazon Pinpoint SMS and Voice Service has no service\-defined resources that can be used as the `Resource` element of an IAM policy statement\.

## Condition Keys for Amazon Pinpoint SMS and Voice Service<a name="amazonpinpointsmsandvoiceservice-policy-keys"></a>

Pinpoint SMS Voice has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available Keys for Conditions](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.