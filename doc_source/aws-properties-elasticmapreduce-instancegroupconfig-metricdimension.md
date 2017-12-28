# Amazon EMR InstanceGroupConfig MetricDimension<a name="aws-properties-elasticmapreduce-instancegroupconfig-metricdimension"></a>

The `MetricDimension` property type represents a CloudWatch dimension that you specify using a key–value pair\. The `Dimensions` subproperty of the [Amazon EMR InstanceGroupConfig CloudWatchAlarmDefinition](aws-properties-elasticmapreduce-instancegroupconfig-cloudwatchalarmdefinition.md) property contains a list of one or more `MetricDimension` property types\.

## Syntax<a name="w3ab2c21c14d994b5"></a>

### JSON<a name="aws-properties-elasticmapreduce-instancegroupconfig-metricdimension-syntax.json"></a>

```
{
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-elasticmapreduce-instancegroupconfig-metricdimension-key)" : String,
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-elasticmapreduce-instancegroupconfig-metricdimension-value)" : String
}
```

### YAML<a name="aws-properties-elasticmapreduce-instancegroupconfig-metricdimension-syntax.yaml"></a>

```
  [[ERROR] BAD/MISSING LINK TEXT](#cfn-elasticmapreduce-instancegroupconfig-metricdimension-key): String
  [[ERROR] BAD/MISSING LINK TEXT](#cfn-elasticmapreduce-instancegroupconfig-metricdimension-value): String
```

## Properties<a name="w3ab2c21c14d994b7"></a>

By default, Amazon EMR uses one dimension whose key \(known as a `Name` in CloudWatch\) is `JobFlowID` and whose value is a variable representing the cluster ID, which is `${emr.clusterId}`\. This enables the rule to bootstrap when the cluster ID becomes available\.

`Key`  
The dimension name\.  
*Required: *Yes  
*Type*: String

`Value`  
The dimension value\.  
*Required: *Yes  
*Type*: String