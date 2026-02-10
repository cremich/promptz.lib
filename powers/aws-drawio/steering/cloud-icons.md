# Cloud Provider Icons Reference

Draw.io has built-in shape libraries for AWS, Azure, and GCP. This reference covers the mxCell syntax for using official cloud icons.

## Table of Contents

1. [AWS Icons (aws4)](#aws-icons-aws4)
2. [Azure Icons (azure2)](#azure-icons-azure2)
3. [GCP Icons](#gcp-icons)
4. [AWS Groups and Containers](#aws-groups-and-containers)
5. [Usage Tips](#usage-tips)

---

## AWS Icons (aws4)

AWS icons use the `mxgraph.aws4` shape library with the `resourceIcon` shape type.

### Base Style Template

```xml
<mxCell id="unique-id" value="Label" style="sketch=0;points=[[0,0,0],[0.25,0,0],[0.5,0,0],[0.75,0,0],[1,0,0],[0,1,0],[0.25,1,0],[0.5,1,0],[0.75,1,0],[1,1,0],[0,0.25,0],[0,0.5,0],[0,0.75,0],[1,0.25,0],[1,0.5,0],[1,0.75,0]];outlineConnect=0;fontColor=#232F3E;fillColor=#COLOR;strokeColor=#ffffff;dashed=0;verticalLabelPosition=bottom;verticalAlign=top;align=center;html=1;fontSize=12;fontStyle=0;aspect=fixed;shape=mxgraph.aws4.resourceIcon;resIcon=mxgraph.aws4.SERVICE_NAME;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="78" height="78" as="geometry" />
</mxCell>
```

### AWS Service Categories and Colors

| Category | fillColor | Services |
|----------|-----------|----------|
| Compute | #ED7100 | ec2, lambda, ecs, eks, fargate, batch |
| Storage | #7AA116 | s3, ebs, efs, fsx, storage_gateway |
| Database | #C925D1 | rds, dynamodb, elasticache, redshift, neptune, documentdb |
| Networking | #8C4FFF | vpc, cloudfront, route53, api_gateway, elb, direct_connect |
| Security | #DD344C | iam, cognito, secrets_manager, kms, waf, shield |
| Management | #E7157B | cloudwatch, cloudformation, systems_manager, config |
| Analytics | #8C4FFF | kinesis, athena, emr, glue, quicksight |
| Application | #E7157B | sns, sqs, step_functions, eventbridge |
| Migration | #7AA116 | migration_hub, dms, datasync |

### Common AWS Service Icons

#### Compute
```xml
<!-- EC2 -->
resIcon=mxgraph.aws4.ec2;fillColor=#ED7100

<!-- Lambda -->
resIcon=mxgraph.aws4.lambda;fillColor=#ED7100

<!-- ECS -->
resIcon=mxgraph.aws4.ecs;fillColor=#ED7100

<!-- EKS -->
resIcon=mxgraph.aws4.eks;fillColor=#ED7100

<!-- Fargate -->
resIcon=mxgraph.aws4.fargate;fillColor=#ED7100
```

#### Storage
```xml
<!-- S3 -->
resIcon=mxgraph.aws4.s3;fillColor=#7AA116

<!-- EBS -->
resIcon=mxgraph.aws4.elastic_block_store;fillColor=#7AA116

<!-- EFS -->
resIcon=mxgraph.aws4.elastic_file_system;fillColor=#7AA116
```

#### Database
```xml
<!-- RDS -->
resIcon=mxgraph.aws4.rds;fillColor=#C925D1

<!-- DynamoDB -->
resIcon=mxgraph.aws4.dynamodb;fillColor=#C925D1

<!-- ElastiCache -->
resIcon=mxgraph.aws4.elasticache;fillColor=#C925D1

<!-- Aurora -->
resIcon=mxgraph.aws4.aurora;fillColor=#C925D1

<!-- Redshift -->
resIcon=mxgraph.aws4.redshift;fillColor=#C925D1
```

#### Networking
```xml
<!-- VPC -->
resIcon=mxgraph.aws4.vpc;fillColor=#8C4FFF

<!-- CloudFront -->
resIcon=mxgraph.aws4.cloudfront;fillColor=#8C4FFF

<!-- Route 53 -->
resIcon=mxgraph.aws4.route_53;fillColor=#8C4FFF

<!-- API Gateway -->
resIcon=mxgraph.aws4.api_gateway;fillColor=#E7157B

<!-- ELB / ALB -->
resIcon=mxgraph.aws4.elastic_load_balancing;fillColor=#8C4FFF

<!-- Direct Connect -->
resIcon=mxgraph.aws4.direct_connect;fillColor=#8C4FFF

<!-- Transit Gateway -->
resIcon=mxgraph.aws4.transit_gateway;fillColor=#8C4FFF
```

#### Security & Identity
```xml
<!-- IAM -->
resIcon=mxgraph.aws4.identity_and_access_management;fillColor=#DD344C

<!-- Cognito -->
resIcon=mxgraph.aws4.cognito;fillColor=#DD344C

<!-- Secrets Manager -->
resIcon=mxgraph.aws4.secrets_manager;fillColor=#DD344C

<!-- KMS -->
resIcon=mxgraph.aws4.key_management_service;fillColor=#DD344C

<!-- WAF -->
resIcon=mxgraph.aws4.waf;fillColor=#DD344C

<!-- Shield -->
resIcon=mxgraph.aws4.shield;fillColor=#DD344C
```

#### Management & Monitoring
```xml
<!-- CloudWatch -->
resIcon=mxgraph.aws4.cloudwatch;fillColor=#E7157B

<!-- CloudFormation -->
resIcon=mxgraph.aws4.cloudformation;fillColor=#E7157B

<!-- Systems Manager -->
resIcon=mxgraph.aws4.systems_manager;fillColor=#E7157B

<!-- Config -->
resIcon=mxgraph.aws4.config;fillColor=#E7157B
```

#### Application Integration
```xml
<!-- SNS -->
resIcon=mxgraph.aws4.sns;fillColor=#E7157B

<!-- SQS -->
resIcon=mxgraph.aws4.sqs;fillColor=#E7157B

<!-- Step Functions -->
resIcon=mxgraph.aws4.step_functions;fillColor=#E7157B

<!-- EventBridge -->
resIcon=mxgraph.aws4.eventbridge;fillColor=#E7157B
```

#### Migration & Transfer
```xml
<!-- Database Migration Service -->
resIcon=mxgraph.aws4.database_migration_service;fillColor=#7AA116

<!-- DataSync -->
resIcon=mxgraph.aws4.datasync;fillColor=#7AA116

<!-- Migration Hub -->
resIcon=mxgraph.aws4.migration_hub;fillColor=#7AA116
```

### Complete AWS Icon Example

```xml
<mxCell id="aws-lambda-1" value="Lambda Function" style="sketch=0;points=[[0,0,0],[0.25,0,0],[0.5,0,0],[0.75,0,0],[1,0,0],[0,1,0],[0.25,1,0],[0.5,1,0],[0.75,1,0],[1,1,0],[0,0.25,0],[0,0.5,0],[0,0.75,0],[1,0.25,0],[1,0.5,0],[1,0.75,0]];outlineConnect=0;fontColor=#232F3E;fillColor=#ED7100;strokeColor=#ffffff;dashed=0;verticalLabelPosition=bottom;verticalAlign=top;align=center;html=1;fontSize=12;fontStyle=0;aspect=fixed;shape=mxgraph.aws4.resourceIcon;resIcon=mxgraph.aws4.lambda;" vertex="1" parent="1">
  <mxGeometry x="200" y="200" width="78" height="78" as="geometry" />
</mxCell>
```

---

## Azure Icons (azure2)

Azure icons use the `img/lib/azure2/` image path syntax.

### Base Style Template

```xml
<mxCell id="unique-id" value="Label" style="aspect=fixed;html=1;points=[];align=center;image;fontSize=12;image=img/lib/azure2/CATEGORY/SERVICE_NAME.svg;verticalLabelPosition=bottom;verticalAlign=top;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="68" height="68" as="geometry" />
</mxCell>
```

### Azure Service Categories

| Category Path | Services |
|---------------|----------|
| compute | Virtual_Machine, App_Services, Function_Apps, Container_Instances, Kubernetes_Services |
| databases | SQL_Database, Cosmos_DB, SQL_Managed_Instance, Database_PostgreSQL, Cache_Redis |
| storage | Storage_Accounts, Blob_Storage, Data_Lake_Storage, File_Storage |
| networking | Virtual_Networks, Load_Balancers, Application_Gateway, VPN_Gateway, DNS_Zones, CDN_Profiles |
| security | Key_Vaults, Azure_Active_Directory, Security_Center |
| management_governance | Monitor, Log_Analytics_Workspaces, Application_Insights, Automation_Accounts |
| integration | Logic_Apps, Service_Bus, Event_Grid, API_Management |
| ai_machine_learning | Cognitive_Services, Machine_Learning, Bot_Services |

### Common Azure Service Icons

#### Compute
```xml
<!-- Virtual Machine -->
image=img/lib/azure2/compute/Virtual_Machine.svg

<!-- App Service -->
image=img/lib/azure2/app_services/App_Services.svg

<!-- Function App -->
image=img/lib/azure2/compute/Function_Apps.svg

<!-- AKS -->
image=img/lib/azure2/containers/Kubernetes_Services.svg

<!-- Container Instance -->
image=img/lib/azure2/containers/Container_Instances.svg
```

#### Storage
```xml
<!-- Storage Account -->
image=img/lib/azure2/storage/Storage_Accounts.svg

<!-- Blob Storage -->
image=img/lib/azure2/storage/Blob_Storage.svg

<!-- File Storage -->
image=img/lib/azure2/storage/File_Storage.svg

<!-- Data Lake -->
image=img/lib/azure2/storage/Data_Lake_Storage.svg
```

#### Database
```xml
<!-- SQL Database -->
image=img/lib/azure2/databases/SQL_Database.svg

<!-- Cosmos DB -->
image=img/lib/azure2/databases/Azure_Cosmos_DB.svg

<!-- PostgreSQL -->
image=img/lib/azure2/databases/Azure_Database_PostgreSQL_Server.svg

<!-- Redis Cache -->
image=img/lib/azure2/databases/Cache_Redis.svg
```

#### Networking
```xml
<!-- Virtual Network -->
image=img/lib/azure2/networking/Virtual_Networks.svg

<!-- Load Balancer -->
image=img/lib/azure2/networking/Load_Balancers.svg

<!-- Application Gateway -->
image=img/lib/azure2/networking/Application_Gateways.svg

<!-- VPN Gateway -->
image=img/lib/azure2/networking/VPN_Gateways.svg

<!-- Front Door -->
image=img/lib/azure2/networking/Front_Doors.svg

<!-- DNS Zone -->
image=img/lib/azure2/networking/DNS_Zones.svg

<!-- ExpressRoute -->
image=img/lib/azure2/networking/ExpressRoute_Circuits.svg
```

#### Security & Identity
```xml
<!-- Azure AD -->
image=img/lib/azure2/identity/Azure_Active_Directory.svg

<!-- Key Vault -->
image=img/lib/azure2/security/Key_Vaults.svg

<!-- Security Center -->
image=img/lib/azure2/security/Security_Center.svg
```

#### Management & Monitoring
```xml
<!-- Monitor -->
image=img/lib/azure2/management_governance/Monitor.svg

<!-- Log Analytics -->
image=img/lib/azure2/management_governance/Log_Analytics_Workspaces.svg

<!-- Application Insights -->
image=img/lib/azure2/management_governance/Application_Insights.svg

<!-- Automation -->
image=img/lib/azure2/management_governance/Automation_Accounts.svg
```

#### Integration
```xml
<!-- Logic Apps -->
image=img/lib/azure2/integration/Logic_Apps.svg

<!-- Service Bus -->
image=img/lib/azure2/integration/Service_Bus.svg

<!-- Event Grid -->
image=img/lib/azure2/integration/Event_Grid_Domains.svg

<!-- API Management -->
image=img/lib/azure2/integration/API_Management_Services.svg
```

### Complete Azure Icon Example

```xml
<mxCell id="azure-vm-1" value="Web Server" style="aspect=fixed;html=1;points=[];align=center;image;fontSize=12;image=img/lib/azure2/compute/Virtual_Machine.svg;verticalLabelPosition=bottom;verticalAlign=top;" vertex="1" parent="1">
  <mxGeometry x="200" y="200" width="68" height="68" as="geometry" />
</mxCell>
```

---

## GCP Icons

GCP icons use the `img/lib/google/` image path.

### Base Style Template

```xml
<mxCell id="unique-id" value="Label" style="aspect=fixed;html=1;points=[];align=center;image;fontSize=12;image=img/lib/google/CATEGORY/SERVICE_NAME.svg;verticalLabelPosition=bottom;verticalAlign=top;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="68" height="68" as="geometry" />
</mxCell>
```

### Common GCP Icons

```xml
<!-- Compute Engine -->
image=img/lib/google/compute/Compute_Engine.svg

<!-- Cloud Functions -->
image=img/lib/google/serverless/Cloud_Functions.svg

<!-- GKE -->
image=img/lib/google/containers/Kubernetes_Engine.svg

<!-- Cloud Storage -->
image=img/lib/google/storage/Cloud_Storage.svg

<!-- Cloud SQL -->
image=img/lib/google/databases/Cloud_SQL.svg

<!-- BigQuery -->
image=img/lib/google/big_data/BigQuery.svg

<!-- VPC -->
image=img/lib/google/networking/Virtual_Private_Cloud.svg

<!-- Load Balancer -->
image=img/lib/google/networking/Cloud_Load_Balancing.svg
```

---

## AWS Groups and Containers

AWS diagrams commonly use group shapes to represent regions, VPCs, subnets, etc.

### AWS Cloud Container

```xml
<mxCell id="aws-cloud" value="AWS Cloud" style="sketch=0;outlineConnect=0;gradientColor=none;html=1;whiteSpace=wrap;fontSize=12;fontStyle=0;shape=mxgraph.aws4.group;grIcon=mxgraph.aws4.group_aws_cloud;strokeColor=#AAB7B8;fillColor=none;verticalAlign=top;align=left;spacingLeft=30;fontColor=#AAB7B8;dashed=0;" vertex="1" parent="1">
  <mxGeometry x="40" y="40" width="600" height="400" as="geometry" />
</mxCell>
```

### Region Container

```xml
<mxCell id="aws-region" value="eu-west-2" style="sketch=0;outlineConnect=0;gradientColor=none;html=1;whiteSpace=wrap;fontSize=12;fontStyle=0;shape=mxgraph.aws4.group;grIcon=mxgraph.aws4.group_region;strokeColor=#00A4A6;fillColor=none;verticalAlign=top;align=left;spacingLeft=30;fontColor=#007F7F;dashed=1;" vertex="1" parent="1">
  <mxGeometry x="60" y="80" width="520" height="340" as="geometry" />
</mxCell>
```

### VPC Container

```xml
<mxCell id="aws-vpc" value="VPC" style="sketch=0;outlineConnect=0;gradientColor=none;html=1;whiteSpace=wrap;fontSize=12;fontStyle=0;shape=mxgraph.aws4.group;grIcon=mxgraph.aws4.group_vpc;strokeColor=#8C4FFF;fillColor=none;verticalAlign=top;align=left;spacingLeft=30;fontColor=#AAB7B8;dashed=0;" vertex="1" parent="1">
  <mxGeometry x="80" y="120" width="460" height="280" as="geometry" />
</mxCell>
```

### Public Subnet

```xml
<mxCell id="public-subnet" value="Public Subnet" style="sketch=0;outlineConnect=0;gradientColor=none;html=1;whiteSpace=wrap;fontSize=12;fontStyle=0;shape=mxgraph.aws4.group;grIcon=mxgraph.aws4.group_public_subnet;strokeColor=#7AA116;fillColor=#E9F3E6;verticalAlign=top;align=left;spacingLeft=30;fontColor=#248814;dashed=0;" vertex="1" parent="1">
  <mxGeometry x="100" y="160" width="200" height="200" as="geometry" />
</mxCell>
```

### Private Subnet

```xml
<mxCell id="private-subnet" value="Private Subnet" style="sketch=0;outlineConnect=0;gradientColor=none;html=1;whiteSpace=wrap;fontSize=12;fontStyle=0;shape=mxgraph.aws4.group;grIcon=mxgraph.aws4.group_private_subnet;strokeColor=#00A4A6;fillColor=#E6F6F7;verticalAlign=top;align=left;spacingLeft=30;fontColor=#147EBA;dashed=0;" vertex="1" parent="1">
  <mxGeometry x="320" y="160" width="200" height="200" as="geometry" />
</mxCell>
```

### Availability Zone

```xml
<mxCell id="az-1" value="Availability Zone 1" style="sketch=0;outlineConnect=0;gradientColor=none;html=1;whiteSpace=wrap;fontSize=12;fontStyle=0;shape=mxgraph.aws4.group;grIcon=mxgraph.aws4.group_availability_zone;strokeColor=#00A4A6;fillColor=none;verticalAlign=top;align=left;spacingLeft=30;fontColor=#007F7F;dashed=1;" vertex="1" parent="1">
  <mxGeometry x="100" y="160" width="200" height="200" as="geometry" />
</mxCell>
```

### Security Group

```xml
<mxCell id="security-group" value="Security Group" style="sketch=0;outlineConnect=0;gradientColor=none;html=1;whiteSpace=wrap;fontSize=12;fontStyle=0;shape=mxgraph.aws4.group;grIcon=mxgraph.aws4.group_security_group;strokeColor=#DD344C;fillColor=#FFEBEE;verticalAlign=top;align=left;spacingLeft=30;fontColor=#DD344C;dashed=0;" vertex="1" parent="1">
  <mxGeometry x="120" y="200" width="160" height="140" as="geometry" />
</mxCell>
```

---

## Usage Tips

### Enabling Libraries in draw.io

To access AWS/Azure icons in draw.io:
1. Click **More Shapes** at bottom of shapes panel
2. Expand **Networking** section
3. Enable **AWS 2019** / **AWS 2021** / **Azure** / **GCP** libraries
4. Click **Apply**

Alternatively, open draw.io with libraries pre-loaded:
- AWS: `https://app.diagrams.net/?libs=aws4`
- Azure: `https://app.diagrams.net/?libs=azure2`

### Icon Sizing

| Standard Size | Use Case |
|---------------|----------|
| 48x48 | Compact diagrams |
| 64x64 | Standard diagrams |
| 78x78 | AWS default |
| 96x96 | Large/detailed diagrams |

### Label Positioning

```xml
<!-- Label below icon -->
verticalLabelPosition=bottom;verticalAlign=top;

<!-- Label to the right -->
labelPosition=right;align=left;verticalAlign=middle;

<!-- No label (icon only) -->
value=""
```

### Finding Icon Names

If unsure of exact icon name:
1. Open draw.io with the relevant library enabled
2. Drag the icon onto canvas
3. Select it and press Ctrl+E (or Cmd+E on Mac) to view style
4. Copy the `resIcon=` or `image=` value

### Mixing Providers

When creating multi-cloud diagrams, maintain visual consistency:
- Use similar icon sizes across providers
- Group each cloud in its own container
- Use provider-specific colours for containers
- Add a legend showing provider colors
