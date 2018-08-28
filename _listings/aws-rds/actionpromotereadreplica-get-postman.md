{
  "info": {
    "name": "Amazon RDS API Promote Read Replica",
    "_postman_id": "19e94b0a-2b9d-417e-b55d-076b7845f4c5",
    "description": "Promotes a Read Replica DB instance to a standalone DB instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "abbea3c9-21d8-4f0c-8f5f-b7d09fa686b8",
          "name": "addroletodbcluster",
          "request": {
            "url": "http://example.com/api/?Action=AddRoleToDBCluster?DBClusterIdentifier=DBClusterIdentifier&RoleArn=RoleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates an Identity and Access Management (IAM) role from an Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66e2980a-42bf-483f-b6f1-0845d3cdf6fe"
            }
          ]
        },
        {
          "id": "0a8db3d7-7440-4295-a629-d4397fc50fb7",
          "name": "createdbcluster",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBCluster?AvailabilityZones.AvailabilityZone.N=AvailabilityZones.AvailabilityZone.N&BackupRetentionPeriod=BackupRetentionPeriod&CharacterSetName=CharacterSetName&DatabaseName=DatabaseName&DBClusterIdentifier=DBClusterIdentifier&DBClusterParameterGroupName=DBClusterParameterGroupName&DBSubnetGroupName=DBSubnetGroupName&Engine=Engine&EngineVersion=EngineVersion&KmsKeyId=KmsKeyId&MasterUsername=MasterUsername&MasterUserPassword=MasterUserPassword&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&ReplicationSourceIdentifier=ReplicationSourceIdentifier&StorageEncrypted=StorageEncrypted&Tags.Tag.N=Tags.Tag.N&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "770f0791-5c5b-4251-9814-0abdfd6c3a7b"
            }
          ]
        },
        {
          "id": "3417802a-b580-42cf-80e0-2a7f0155756b",
          "name": "deletedbcluster",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBCluster?DBClusterIdentifier=DBClusterIdentifier&FinalDBSnapshotIdentifier=FinalDBSnapshotIdentifier&SkipFinalSnapshot=SkipFinalSnapshot",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteDBCluster action deletes a previously provisioned DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6a87b54-acf4-42cb-827a-020e37d4be92"
            }
          ]
        },
        {
          "id": "dc44b23a-f4ac-47ab-9c30-fa24c2d0ea4a",
          "name": "describedbclusters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusters?DBClusterIdentifier=DBClusterIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about provisioned Aurora DB clusters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ae39b25-63b0-4e67-8e82-c6409025edfc"
            }
          ]
        },
        {
          "id": "4637de31-9914-4185-bcb6-0021e71bf773",
          "name": "failoverdbcluster",
          "request": {
            "url": "http://example.com/api/?Action=FailoverDBCluster?DBClusterIdentifier=DBClusterIdentifier&TargetDBInstanceIdentifier=TargetDBInstanceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Forces a failover for a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "294084bc-f610-4f19-b6c7-cb843f8b5618"
            }
          ]
        },
        {
          "id": "dd9b884e-c42d-4bed-96f7-9cc99066ac70",
          "name": "modifydbcluster",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBCluster?ApplyImmediately=ApplyImmediately&BackupRetentionPeriod=BackupRetentionPeriod&DBClusterIdentifier=DBClusterIdentifier&DBClusterParameterGroupName=DBClusterParameterGroupName&MasterUserPassword=MasterUserPassword&NewDBClusterIdentifier=NewDBClusterIdentifier&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modify a setting for an Amazon Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "865a733c-e37b-4b23-8150-f729fea724bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "0746517d-59f4-4251-a50c-caa5f6de4591",
          "name": "addsourceidentifiertosubscription",
          "request": {
            "url": "http://example.com/api/?Action=AddSourceIdentifierToSubscription?SourceIdentifier=SourceIdentifier&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a source identifier to an existing RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc58e1cc-4674-42b0-bdf3-8182fd720728"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "a2ac8654-737b-4531-8a5c-27b88dc30d9a",
          "name": "addtagstoresource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceName=ResourceName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds metadata tags to an Amazon RDS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22505259-4b54-40be-a00f-840ec4bdc720"
            }
          ]
        },
        {
          "id": "c3fa2b12-9319-4563-818b-ca8b1016bbe9",
          "name": "listtagsforresource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?Filters.Filter.N=Filters.Filter.N&ResourceName=ResourceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all tags on an Amazon RDS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d1a8e18-419c-4b2a-b5e3-866a5548f7ac"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance Actions",
      "item": [
        {
          "id": "1f66ee3b-f395-48df-b385-0dc9a00b72d4",
          "name": "applypendingmaintenanceaction",
          "request": {
            "url": "http://example.com/api/?Action=ApplyPendingMaintenanceAction?ApplyAction=ApplyAction&OptInType=OptInType&ResourceIdentifier=ResourceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a pending maintenance action to a resource (for example, to a DB instance)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa28ace5-19fa-4a48-a1f4-33f00ff6869b"
            }
          ]
        },
        {
          "id": "1f1f5aa6-9eef-4a20-8786-a87a9332a37a",
          "name": "describependingmaintenanceactions",
          "request": {
            "url": "http://example.com/api/?Action=DescribePendingMaintenanceActions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&ResourceIdentifier=ResourceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of resources (for example, DB instances) that have at least one pending maintenance action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a42c288a-5b65-4809-b799-c10e87a3f36d"
            }
          ]
        }
      ]
    },
    {
      "name": "Security Groups",
      "item": [
        {
          "id": "e695dce8-9486-4f33-b98f-eed699851064",
          "name": "authorizedbsecuritygroupingress",
          "request": {
            "url": "http://example.com/api/?Action=AuthorizeDBSecurityGroupIngress?CIDRIP=CIDRIP&DBSecurityGroupName=DBSecurityGroupName&EC2SecurityGroupId=EC2SecurityGroupId&EC2SecurityGroupName=EC2SecurityGroupName&EC2SecurityGroupOwnerId=EC2SecurityGroupOwnerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables ingress to a DBSecurityGroup using one of two forms of authorization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2dba6db3-51ce-4fbb-8be4-bb7147c15cd1"
            }
          ]
        },
        {
          "id": "ba14e780-8ad7-4eeb-b92d-55755857a3cc",
          "name": "createdbsecuritygroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSecurityGroup?DBSecurityGroupDescription=DBSecurityGroupDescription&DBSecurityGroupName=DBSecurityGroupName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "917857e7-e6c3-49f3-86f8-12b071139db6"
            }
          ]
        },
        {
          "id": "084d0d79-2aff-415b-924a-6bc9a9f95b72",
          "name": "deletedbsecuritygroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSecurityGroup?DBSecurityGroupName=DBSecurityGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d69aeedf-23c3-496c-b285-4f7460f79948"
            }
          ]
        },
        {
          "id": "a72f75fe-f966-4438-8168-051e1f311e10",
          "name": "describedbsecuritygroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSecurityGroups?DBSecurityGroupName=DBSecurityGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBSecurityGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2c3a51b-d256-4610-85af-bcb093db6f19"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameter Groups",
      "item": [
        {
          "id": "a400cc9c-bdff-4a03-bec7-0421e4bab162",
          "name": "copydbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBClusterParameterGroup?SourceDBClusterParameterGroupIdentifier=SourceDBClusterParameterGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBClusterParameterGroupDescription=TargetDBClusterParameterGroupDescription&TargetDBClusterParameterGroupIdentifier=TargetDBClusterParameterGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36d11630-b6f9-4f45-8f1c-516ea008b491"
            }
          ]
        },
        {
          "id": "49b4ec7b-7d59-4b07-ab23-2337d7b0d5fa",
          "name": "createdbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName&DBParameterGroupFamily=DBParameterGroupFamily&Description=Description&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "659077b6-01ab-4a0c-adb8-f14c557464cf"
            }
          ]
        },
        {
          "id": "6569476f-afa2-4ef0-9e52-c47d56c19c56",
          "name": "deletedbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50128f19-df27-4841-b220-37e18b7c66ec"
            }
          ]
        },
        {
          "id": "47830e0d-0e0e-4122-9b67-1ac7c0e3e0ec",
          "name": "describedbclusterparametergroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterParameterGroups?DBClusterParameterGroupName=DBClusterParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBClusterParameterGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43ef2c2a-aaa1-4d5e-b082-a153878ee86e"
            }
          ]
        },
        {
          "id": "33c7f634-6a7a-48d9-a480-043c6efd8f7c",
          "name": "modifydbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName&Parameters.Parameter.N=Parameters.Parameter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the parameters of a DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "826cc86a-9670-44fa-b1ae-97a23c4c5733"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Snapshots",
      "item": [
        {
          "id": "8b0b332f-69e5-4ec9-acb5-25268715b652",
          "name": "copydbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBClusterSnapshot?SourceDBClusterSnapshotIdentifier=SourceDBClusterSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBClusterSnapshotIdentifier=TargetDBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f841e7b-a46a-44b7-8b66-00ca3d719db6"
            }
          ]
        },
        {
          "id": "0e674b75-cc1c-4ec1-9a01-3dbf743ec8cf",
          "name": "createdbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBClusterSnapshot?DBClusterIdentifier=DBClusterIdentifier&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19b182d7-dc0f-4e34-bf06-03b0ef376cf5"
            }
          ]
        },
        {
          "id": "4d095e81-54fb-42a2-8a9b-84afd607c476",
          "name": "deletedbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBClusterSnapshot?DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8344637-05bc-4c86-ab40-3a34e4f0c942"
            }
          ]
        },
        {
          "id": "a04af58a-1363-4b56-af5d-7ef0b61d875f",
          "name": "describedbclustersnapshotattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterSnapshotAttributes?DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB cluster snapshot attribute names and values for a manual DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e591769-bfde-4a82-b5e6-c383425ed180"
            }
          ]
        },
        {
          "id": "7464c31c-67f8-4f5c-88d4-4ea07fb6abb9",
          "name": "describedbclustersnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterSnapshots?DBClusterIdentifier=DBClusterIdentifier&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&Filters.Filter.N=Filters.Filter.N&IncludePublic=IncludePublic&IncludeShared=IncludeShared&Marker=Marker&MaxRecords=MaxRecords&SnapshotType=SnapshotType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about DB cluster snapshots."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23c847ec-6cd6-4987-a55f-411c2af40121"
            }
          ]
        },
        {
          "id": "ab17d52b-c08f-4804-be89-9b0e19139d5c",
          "name": "modifydbclustersnapshotattribute",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBClusterSnapshotAttribute?AttributeName=AttributeName&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&ValuesToAdd.AttributeValue.N=ValuesToAdd.AttributeValue.N&ValuesToRemove.AttributeValue.N=ValuesToRemove.AttributeValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an attribute and values to, or removes an attribute and values from, a manual DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cd4899b-8650-47e9-8ea4-967fdaf8a6f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter Groups",
      "item": [
        {
          "id": "673fab38-3fc0-492b-8246-1e1bed8e951b",
          "name": "copydbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBParameterGroup?SourceDBParameterGroupIdentifier=SourceDBParameterGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBParameterGroupDescription=TargetDBParameterGroupDescription&TargetDBParameterGroupIdentifier=TargetDBParameterGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2389e463-9827-4f64-862f-a781d69e4735"
            }
          ]
        },
        {
          "id": "68eb1b4d-9ef2-44c3-ba5d-645ae1a20406",
          "name": "createdbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBParameterGroup?DBParameterGroupFamily=DBParameterGroupFamily&DBParameterGroupName=DBParameterGroupName&Description=Description&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01f88b3a-c7b9-4a23-8fb4-1ae5e6939f03"
            }
          ]
        },
        {
          "id": "5123d46a-a133-475f-89c3-923119cadebd",
          "name": "deletedbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBParameterGroup?DBParameterGroupName=DBParameterGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified DBParameterGroup."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f4b159e-9854-42c7-abf2-72e0b5d06aa7"
            }
          ]
        },
        {
          "id": "392e5a16-40aa-4f28-9895-24727f7b7491",
          "name": "describedbparametergroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBParameterGroups?DBParameterGroupName=DBParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBParameterGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "524f3f75-cec6-4a98-a742-2fc24a498755"
            }
          ]
        },
        {
          "id": "ab945286-5f59-4f54-b4c6-2410816f2abe",
          "name": "modifydbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBParameterGroup?DBParameterGroupName=DBParameterGroupName&Parameters.Parameter.N=Parameters.Parameter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the parameters of a DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6f35820-7c16-41db-b0d8-66ad5532edfb"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "1f006792-8b73-4a67-a1d8-43047197b26b",
          "name": "copydbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBSnapshot?CopyTags=CopyTags&KmsKeyId=KmsKeyId&PreSignedUrl=PreSignedUrl&SourceDBSnapshotIdentifier=SourceDBSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBSnapshotIdentifier=TargetDBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3efdf7ef-4f78-43d3-aca3-c6830cd1b8d3"
            }
          ]
        },
        {
          "id": "cac6df9e-260e-49b0-801b-e0558dda72d7",
          "name": "createdbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSnapshot?DBInstanceIdentifier=DBInstanceIdentifier&DBSnapshotIdentifier=DBSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a DBSnapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cd33737-0805-4fd0-a8dc-92882421803e"
            }
          ]
        },
        {
          "id": "fac293be-cf17-4f55-81f7-d38e3170eca8",
          "name": "deletedbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSnapshot?DBSnapshotIdentifier=DBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DBSnapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "609ac414-9bf6-41c8-add2-29a5bcc3803f"
            }
          ]
        },
        {
          "id": "35e2a598-f7fd-43ee-8240-db2d745b6b1d",
          "name": "describedbsnapshotattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSnapshotAttributes?DBSnapshotIdentifier=DBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB snapshot attribute names and values for a manual DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd679647-72c6-41a8-b8eb-d5e4ae1c86b8"
            }
          ]
        },
        {
          "id": "fe8ddc8b-70c3-4afc-b63c-0955dc56ab46",
          "name": "describedbsnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSnapshots?DBInstanceIdentifier=DBInstanceIdentifier&DBSnapshotIdentifier=DBSnapshotIdentifier&Filters.Filter.N=Filters.Filter.N&IncludePublic=IncludePublic&IncludeShared=IncludeShared&Marker=Marker&MaxRecords=MaxRecords&SnapshotType=SnapshotType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about DB snapshots."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b27421bf-299b-44c4-a8ae-517516da489f"
            }
          ]
        },
        {
          "id": "776abcad-6e7c-4458-845e-3aa9619700cb",
          "name": "modifydbsnapshotattribute",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBSnapshotAttribute?AttributeName=AttributeName&DBSnapshotIdentifier=DBSnapshotIdentifier&ValuesToAdd.AttributeValue.N=ValuesToAdd.AttributeValue.N&ValuesToRemove.AttributeValue.N=ValuesToRemove.AttributeValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an attribute and values to, or removes an attribute and values from, a manual DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3dca4fc-9f0e-419f-87f0-77d4da81a355"
            }
          ]
        }
      ]
    },
    {
      "name": "Option Groups",
      "item": [
        {
          "id": "9f6ac4f3-e1c9-418b-854f-f18aaac2d99f",
          "name": "copyoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyOptionGroup?SourceOptionGroupIdentifier=SourceOptionGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetOptionGroupDescription=TargetOptionGroupDescription&TargetOptionGroupIdentifier=TargetOptionGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0b2b87f-27d0-4524-ad36-83220dc96462"
            }
          ]
        },
        {
          "id": "642b9989-0f9e-4734-aaa7-16d122364a4c",
          "name": "createoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateOptionGroup?EngineName=EngineName&MajorEngineVersion=MajorEngineVersion&OptionGroupDescription=OptionGroupDescription&OptionGroupName=OptionGroupName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff4ec4e8-c166-40c0-acf3-c4770ab5eea8"
            }
          ]
        },
        {
          "id": "304dc1cd-c344-44b3-b773-4db527c041ff",
          "name": "deleteoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteOptionGroup?OptionGroupName=OptionGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e1aa97e-fab9-4c9f-b8e9-9cddd4a76b1b"
            }
          ]
        },
        {
          "id": "f81c5044-f93b-4008-8f44-edbfc705bf6b",
          "name": "describeoptiongroupoptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOptionGroupOptions?EngineName=EngineName&Filters.Filter.N=Filters.Filter.N&MajorEngineVersion=MajorEngineVersion&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes all available options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a8c658d-95c0-46dd-bcae-279e9ffece64"
            }
          ]
        },
        {
          "id": "590a3a6f-a318-4dc8-8277-a112eb678ee5",
          "name": "describeoptiongroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOptionGroups?EngineName=EngineName&Filters.Filter.N=Filters.Filter.N&MajorEngineVersion=MajorEngineVersion&Marker=Marker&MaxRecords=MaxRecords&OptionGroupName=OptionGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available option groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "522b4c35-c982-4589-94ad-69490a9eb926"
            }
          ]
        },
        {
          "id": "39a062b1-edd4-43c3-92e6-d157847c664e",
          "name": "modifyoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyOptionGroup?ApplyImmediately=ApplyImmediately&OptionGroupName=OptionGroupName&OptionsToInclude.OptionConfiguration.N=OptionsToInclude.OptionConfiguration.N&OptionsToRemove.member.N=OptionsToRemove.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f56b97ac-c27e-4c6f-8e93-d2169129585c"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "a1266880-2572-40ca-9429-8cc366473fcb",
          "name": "createdbinstance",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBInstance?AllocatedStorage=AllocatedStorage&AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&BackupRetentionPeriod=BackupRetentionPeriod&CharacterSetName=CharacterSetName&CopyTagsToSnapshot=CopyTagsToSnapshot&DBClusterIdentifier=DBClusterIdentifier&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBName=DBName&DBParameterGroupName=DBParameterGroupName&DBSecurityGroups.DBSecurityGroupName.N=DBSecurityGroups.DBSecurityGroupName.N&DBSubnetGroupName=DBSubnetGroupName&Domain=Domain&DomainIAMRoleName=DomainIAMRoleName&Engine=Engine&EngineVersion=EngineVersion&Iops=Iops&KmsKeyId=KmsKeyId&LicenseModel=LicenseModel&MasterUsername=MasterUsername&MasterUserPassword=MasterUserPassword&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&MultiAZ=MultiAZ&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PromotionTier=PromotionTier&PubliclyAccessible=PubliclyAccessible&StorageEncrypted=StorageEncrypted&StorageType=StorageType&Tags.Tag.N=Tags.Tag.N&TdeCredentialArn=TdeCredentialArn&TdeCredentialPassword=TdeCredentialPassword&Timezone=Timezone&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "804d41dc-5321-4dff-a3d6-6ca52126d89f"
            }
          ]
        },
        {
          "id": "01223d59-d46f-4aa2-8835-bff23ca492bb",
          "name": "createdbinstancereadreplica",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBInstanceReadReplica?AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&CopyTagsToSnapshot=CopyTagsToSnapshot&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBSubnetGroupName=DBSubnetGroupName&Iops=Iops&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&OptionGroupName=OptionGroupName&Port=Port&PubliclyAccessible=PubliclyAccessible&SourceDBInstanceIdentifier=SourceDBInstanceIdentifier&StorageType=StorageType&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a DB instance for a DB instance running MySQL, MariaDB, or PostgreSQL that acts as a Read Replica of a source DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c845aa6c-2ee9-46e4-a410-367035ff901d"
            }
          ]
        },
        {
          "id": "dce79b6a-41d4-4b13-864c-05645f71d65c",
          "name": "deletedbinstance",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBInstance?DBInstanceIdentifier=DBInstanceIdentifier&FinalDBSnapshotIdentifier=FinalDBSnapshotIdentifier&SkipFinalSnapshot=SkipFinalSnapshot",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteDBInstance action deletes a previously provisioned DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee42c8a3-c1e2-4c6f-b2e3-bdb3a0af7484"
            }
          ]
        },
        {
          "id": "e3ed1971-e033-49f8-bad0-df2a615c0df7",
          "name": "describedbinstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBInstances?DBInstanceIdentifier=DBInstanceIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about provisioned RDS instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8020be1b-0c6e-4895-a8e5-c9df0cfadd8c"
            }
          ]
        },
        {
          "id": "d68bb67c-9485-4a43-8f16-b32c333c534f",
          "name": "describeorderabledbinstanceoptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOrderableDBInstanceOptions?DBInstanceClass=DBInstanceClass&Engine=Engine&EngineVersion=EngineVersion&Filters.Filter.N=Filters.Filter.N&LicenseModel=LicenseModel&Marker=Marker&MaxRecords=MaxRecords&Vpc=Vpc",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of orderable DB instance options for the specified engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "050f7249-0cbc-4c6c-b414-80293c890499"
            }
          ]
        },
        {
          "id": "cfebe7ba-014d-43a0-bec1-b254f5c3c757",
          "name": "describereserveddbinstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReservedDBInstances?DBInstanceClass=DBInstanceClass&Duration=Duration&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&MultiAZ=MultiAZ&OfferingType=OfferingType&ProductDescription=ProductDescription&ReservedDBInstanceId=ReservedDBInstanceId&ReservedDBInstancesOfferingId=ReservedDBInstancesOfferingId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about reserved DB instances for this account, or about a specified reserved DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a424afbe-8344-40fd-b11a-9d8d4bc059dc"
            }
          ]
        },
        {
          "id": "373498d1-3e80-4a9d-a97c-6105cd6734c5",
          "name": "describereserveddbinstancesofferings",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReservedDBInstancesOfferings?DBInstanceClass=DBInstanceClass&Duration=Duration&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&MultiAZ=MultiAZ&OfferingType=OfferingType&ProductDescription=ProductDescription&ReservedDBInstancesOfferingId=ReservedDBInstancesOfferingId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists available reserved DB instance offerings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a961ef3c-3eb1-45ee-a1cb-872ef0dd4765"
            }
          ]
        },
        {
          "id": "b420a6a0-9fdf-4485-a6ad-6a05d74e3899",
          "name": "modifydbinstance",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBInstance?AllocatedStorage=AllocatedStorage&AllowMajorVersionUpgrade=AllowMajorVersionUpgrade&ApplyImmediately=ApplyImmediately&AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&BackupRetentionPeriod=BackupRetentionPeriod&CACertificateIdentifier=CACertificateIdentifier&CopyTagsToSnapshot=CopyTagsToSnapshot&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBParameterGroupName=DBParameterGroupName&DBPortNumber=DBPortNumber&DBSecurityGroups.DBSecurityGroupName.N=DBSecurityGroups.DBSecurityGroupName.N&DBSubnetGroupName=DBSubnetGroupName&Domain=Domain&DomainIAMRoleName=DomainIAMRoleName&EngineVersion=EngineVersion&Iops=Iops&LicenseModel=LicenseModel&MasterUserPassword=MasterUserPassword&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&MultiAZ=MultiAZ&NewDBInstanceIdentifier=NewDBInstanceIdentifier&OptionGroupName=OptionGroupName&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PromotionTier=PromotionTier&PubliclyAccessible=PubliclyAccessible&StorageType=StorageType&TdeCredentialArn=TdeCredentialArn&TdeCredentialPassword=TdeCredentialPassword&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies settings for a DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41d815d7-078b-40ef-a68d-5481813b84e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Subnet Groups",
      "item": [
        {
          "id": "6ebf8a54-5b75-4291-a848-9ba1b2d3d756",
          "name": "createdbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSubnetGroup?DBSubnetGroupDescription=DBSubnetGroupDescription&DBSubnetGroupName=DBSubnetGroupName&SubnetIds.SubnetIdentifier.N=SubnetIds.SubnetIdentifier.N&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d847d4f3-c442-48bd-873b-fe0bc2cc1e28"
            }
          ]
        },
        {
          "id": "9c12f100-0f4a-4ef3-bd0c-9001c24ca354",
          "name": "deletedbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSubnetGroup?DBSubnetGroupName=DBSubnetGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "583671e5-5a24-4222-9fc3-c808e6ac7f52"
            }
          ]
        },
        {
          "id": "5ccbbc00-9b2d-4d10-9510-cfb827de5720",
          "name": "describedbsubnetgroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSubnetGroups?DBSubnetGroupName=DBSubnetGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBSubnetGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1118ae2f-9aa0-49c1-bf99-b0122ffc77f3"
            }
          ]
        },
        {
          "id": "9f32f1bc-cd80-4e99-829c-8508461eb249",
          "name": "modifydbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBSubnetGroup?DBSubnetGroupDescription=DBSubnetGroupDescription&DBSubnetGroupName=DBSubnetGroupName&SubnetIds.SubnetIdentifier.N=SubnetIds.SubnetIdentifier.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df3a0d7b-9680-4b48-93f3-25e14045e85f"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "0b7d8cb3-62cf-43bb-b844-b06cc89435ca",
          "name": "createeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=CreateEventSubscription?Enabled=Enabled&EventCategories.EventCategory.N=EventCategories.EventCategory.N&SnsTopicArn=SnsTopicArn&SourceIds.SourceId.N=SourceIds.SourceId.N&SourceType=SourceType&SubscriptionName=SubscriptionName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f94c5f9-9a4a-4158-bc4c-9e48b734044f"
            }
          ]
        },
        {
          "id": "71cc20bd-5f6e-4343-b4aa-277cebbb09f4",
          "name": "deleteeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEventSubscription?SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c6e3e4e-83a4-4304-b60a-4ce30d2ee59d"
            }
          ]
        },
        {
          "id": "13b86296-d573-4777-9622-6ce06296a4c8",
          "name": "describeeventsubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventSubscriptions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the subscription descriptions for a customer account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9479680f-8007-46c6-a635-4ec66cfdf5c0"
            }
          ]
        },
        {
          "id": "b89dd456-399a-40b7-ba16-7d515cc2ca6f",
          "name": "modifyeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=ModifyEventSubscription?Enabled=Enabled&EventCategories.EventCategory.N=EventCategories.EventCategory.N&SnsTopicArn=SnsTopicArn&SourceType=SourceType&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "995c92c6-041d-47e5-872e-51b8770222c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "b51ac8d8-1af2-4054-be80-5a2f80abde83",
          "name": "describeaccountattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountAttributes?AccountQuotas.AccountQuota.N=AccountQuotas.AccountQuota.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the attributes for a customer account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf45a996-a5d3-4f3e-a9b0-64618bd01b72"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "d2b26cae-198b-40c2-861e-0d572f7387ec",
          "name": "describecertificates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCertificates?CertificateIdentifier=CertificateIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the set of CA certificates provided by Amazon RDS for this AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd2858de-c2f3-421b-8266-d311926bccfe"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameters",
      "item": [
        {
          "id": "0774ce4e-601f-49a7-a798-dda4e772a976",
          "name": "describedbclusterparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterParameters?DBClusterParameterGroupName=DBClusterParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&Source=Source",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the detailed parameter list for a particular DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e9d1a16-efe9-4a7c-b599-856356e895a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Engines",
      "item": [
        {
          "id": "84b47719-f939-4ebb-a31b-fd00bad21970",
          "name": "describedbengineversions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBEngineVersions?DBParameterGroupFamily=DBParameterGroupFamily&DefaultOnly=DefaultOnly&Engine=Engine&EngineVersion=EngineVersion&Filters.Filter.N=Filters.Filter.N&ListSupportedCharacterSets=ListSupportedCharacterSets&ListSupportedTimezones=ListSupportedTimezones&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available DB engines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db65ac29-d37c-4b5b-96f9-77847dfe2183"
            }
          ]
        }
      ]
    },
    {
      "name": "Blog Files",
      "item": [
        {
          "id": "f6014183-cffa-4eb6-ac1a-ec3ea042bffa",
          "name": "describedblogfiles",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBLogFiles?DBInstanceIdentifier=DBInstanceIdentifier&FileLastWritten=FileLastWritten&FilenameContains=FilenameContains&FileSize=FileSize&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB log files for the DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0366c837-4d8f-4b14-bce6-88c61d115e24"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "058bb3c4-7a13-4721-808c-9760a311abfb",
          "name": "describedbparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBParameters?DBParameterGroupName=DBParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&Source=Source",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the detailed parameter list for a particular DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77cc8f02-9087-4dc6-871d-0645df5b72a5"
            }
          ]
        }
      ]
    },
    {
      "name": "Default Cluster Parameters",
      "item": [
        {
          "id": "af11475c-5bf7-4c7d-b71b-319b2f757cd5",
          "name": "describeenginedefaultclusterparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEngineDefaultClusterParameters?DBParameterGroupFamily=DBParameterGroupFamily&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default engine and system parameter information for the cluster database engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3c4aa21-5ae8-43a6-a647-e59851f6ca7b"
            }
          ]
        }
      ]
    },
    {
      "name": "Default Parameters",
      "item": [
        {
          "id": "04937003-f746-4756-bae2-77aed639d6cc",
          "name": "describeenginedefaultparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEngineDefaultParameters?DBParameterGroupFamily=DBParameterGroupFamily&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default engine and system parameter information for the specified database engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee3d09ec-2847-4303-9669-6b0f3ae26b64"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Categories",
      "item": [
        {
          "id": "3fed559d-e9da-48e5-b82c-1c7e969e16b0",
          "name": "describeeventcategories",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventCategories?Filters.Filter.N=Filters.Filter.N&SourceType=SourceType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Displays a list of categories for all event source types, or, if specified, for a specified source type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0828f03b-70c5-4920-9df3-a66a6bc76a99"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "b902ad51-1b34-476f-b15c-967f7b12a447",
          "name": "describeevents",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEvents?Duration=Duration&EndTime=EndTime&EventCategories.EventCategory.N=EventCategories.EventCategory.N&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&SourceIdentifier=SourceIdentifier&SourceType=SourceType&StartTime=StartTime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns events related to DB instances, DB security groups, DB snapshots, and DB parameter groups for the past 14 days."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49dfea28-5c0d-44c5-b9ed-ad66b12a3d2f"
            }
          ]
        }
      ]
    },
    {
      "name": "Source Regions",
      "item": [
        {
          "id": "1290fd67-9bfc-4139-99d1-be6b2c04518d",
          "name": "describesourceregions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSourceRegions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&RegionName=RegionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the source AWS regions where the current AWS region can create a Read Replica \n            or copy a DB snapshot from."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "140214dc-a908-41ab-8c94-a618adf051c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Log Files",
      "item": [
        {
          "id": "86068f5e-1f6e-4362-a15a-ac7022128967",
          "name": "downloaddblogfileportion",
          "request": {
            "url": "http://example.com/api/?Action=DownloadDBLogFilePortion?DBInstanceIdentifier=DBInstanceIdentifier&LogFileName=LogFileName&Marker=Marker&NumberOfLines=NumberOfLines",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Downloads all or a portion of the specified log file, up to 1 MB in size."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffe18e44-8115-4db7-990c-03ded35e8339"
            }
          ]
        }
      ]
    },
    {
      "name": "Replicas",
      "item": [
        {
          "id": "d492da23-84fd-498b-8cc0-b5c4a4fed072",
          "name": "promotereadreplica",
          "request": {
            "url": "http://example.com/api/?Action=PromoteReadReplica?BackupRetentionPeriod=BackupRetentionPeriod&DBInstanceIdentifier=DBInstanceIdentifier&PreferredBackupWindow=PreferredBackupWindow",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Promotes a Read Replica DB instance to a standalone DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b363aa8d-4658-43c0-a220-4f17a63aa065"
            }
          ]
        }
      ]
    }
  ]
}