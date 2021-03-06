# Actions, Resources, and Condition Keys for Amazon SimpleDB<a name="list_amazonsimpledb"></a>

Amazon SimpleDB \(service prefix: `sdb`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/UsingIAMWithSDB.html) permission policies\.

**Topics**
+ [Actions Defined by Amazon SimpleDB](#amazonsimpledb-actions-as-permissions)
+ [Resources Defined by Amazon SimpleDB](#amazonsimpledb-resources-for-iam-policies)
+ [Condition Keys for Amazon SimpleDB](#amazonsimpledb-policy-keys)

## Actions Defined by Amazon SimpleDB<a name="amazonsimpledb-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access Level | Resource Types \(\*required\) | Condition Keys | Dependent Actions | 
| --- | --- | --- | --- | --- | --- | 
|   [ BatchDeleteAttributes ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_BatchDeleteAttributes.html)  | Performs multiple DeleteAttributes operations in a single call, which reduces round trips and latencies\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ BatchPutAttributes ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_BatchPutAttributes.html)  | With the BatchPutAttributes operation, you can perform multiple PutAttribute operations in a single call\. With the BatchPutAttributes operation, you can perform multiple PutAttribute operations in a single call\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ CreateDomain ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_CreateDomain.html)  | The CreateDomain operation creates a new domain\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ DeleteAttributes ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_DeleteAttributes.html)  | Deletes one or more attributes associated with the item\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ DeleteDomain ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_DeleteDomain.html)  | The DeleteDomain operation deletes a domain\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ DomainMetadata ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_DomainMetadata.html)  | Returns information about the domain, including when the domain was created, the number of items and attributes, and the size of attribute names and values\. | Read |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ GetAttributes ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_GetAttributes.html)  | Returns all of the attributes associated with the item\. | Read |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ ListDomains ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_ListDomains.html)  | Description for ListDomains | List |  |  |  | 
|   [ PutAttributes ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_PutAttributes.html)  | The PutAttributes operation creates or replaces attributes in an item\. | Write |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 
|   [ Select ](https://docs.aws.amazon.com/AmazonSimpleDB/latest/DeveloperGuide/API_Select.html)  | Description for Select | Read |   [ domain\* ](#amazonsimpledb-domain)   |  |  | 

## Resources Defined by Amazon SimpleDB<a name="amazonsimpledb-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#amazonsimpledb-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ domain ](https://docs.aws.amazon.com/sdb/latest/APIReference/DataModel.html)  |  arn:$\{Partition\}:sdb:$\{Region\}:$\{Account\}:domain/$\{DomainName\}  |  | 

## Condition Keys for Amazon SimpleDB<a name="amazonsimpledb-policy-keys"></a>

SimpleDB has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available Keys for Conditions](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.