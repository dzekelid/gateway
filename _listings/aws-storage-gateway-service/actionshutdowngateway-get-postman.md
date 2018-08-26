{
  "info": {
    "name": "AWS Storage Gateway Service API Shutdown Gateway",
    "_postman_id": "246c16aa-12ae-4a4c-b525-ffa8760071a7",
    "description": "Shuts down a gateway.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gateway",
      "item": [
        {
          "id": "c54ac8e6-bafb-4b69-b74a-d5cdc2c356fe",
          "name": "activateGateway",
          "request": {
            "url": "http://example.com/api/?Action=ActivateGateway?ActivationKey=ActivationKey&GatewayName=GatewayName&GatewayRegion=GatewayRegion&GatewayTimezone=GatewayTimezone&GatewayType=GatewayType&MediumChangerType=MediumChangerType&TapeDriveType=TapeDriveType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Activates the gateway you previously deployed on your host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd70e6e3-3a49-4385-99c9-32a4b5b09aed"
            }
          ]
        },
        {
          "id": "4114ba76-d9b8-4867-b303-b2caa8b08ca7",
          "name": "deleteGateway",
          "request": {
            "url": "http://example.com/api/?Action=DeleteGateway?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95d948b5-616b-47e9-8ea9-086d4c0699fa"
            }
          ]
        },
        {
          "id": "a664d5e7-3ab7-4f09-b0f8-19af5081745b",
          "name": "describeGatewayInformation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeGatewayInformation?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metadata about a gateway such as its name, network interfaces, configured\n         time zone, and the state (whether the gateway is running or not)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ab745c5-047b-4854-9170-8cf0bee52ef7"
            }
          ]
        },
        {
          "id": "8c014d0a-59d6-4ee1-a224-84b168d1b9aa",
          "name": "disableGateway",
          "request": {
            "url": "http://example.com/api/?Action=DisableGateway?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables a gateway when the gateway is no longer functioning."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ea85834-3929-4c9d-80c0-b77a49ad0310"
            }
          ]
        },
        {
          "id": "ff79939c-ec64-4d86-9ac2-bf6fae923977",
          "name": "shutdownGateway",
          "request": {
            "url": "http://example.com/api/?Action=ShutdownGateway?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Shuts down a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0ed1c66-71c8-4779-9304-60556519c956"
            }
          ]
        }
      ]
    },
    {
      "name": "Cache",
      "item": [
        {
          "id": "347d4f27-2304-40ec-a14e-77ada1c96413",
          "name": "addCache",
          "request": {
            "url": "http://example.com/api/?Action=AddCache?DiskIds=DiskIds&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures one or more gateway local disks as cache for a cached-volume gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98bfd020-322f-4f12-95ff-b37ad4d726e9"
            }
          ]
        },
        {
          "id": "10b7c0f1-5193-42f8-9b71-a91eb2433c42",
          "name": "describeCache",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCache?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the cache of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22fefdc2-4dd1-4a84-9997-93f8f6f440e5"
            }
          ]
        },
        {
          "id": "39d6c2ee-45f7-4eb8-8c9d-be5eba052563",
          "name": "resetCache",
          "request": {
            "url": "http://example.com/api/?Action=ResetCache?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Resets all cache disks that have encountered a error and makes the disks available\n         for reconfiguration as cache storage."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d93621d9-94c3-4796-b0d1-f35f132bc694"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "056b9f0a-0368-4bfb-a3b2-b35cfb897fae",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceARN=ResourceARN&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds one or more tags to the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a78c0ed2-6079-4dd8-9868-dfacb59b8b67"
            }
          ]
        },
        {
          "id": "e13a5553-2964-45de-a301-27b074135c05",
          "name": "listTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?Limit=Limit&Marker=Marker&ResourceARN=ResourceARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the tags that have been added to the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7490b7d-434e-4e4d-bb02-0eecfbdca99c"
            }
          ]
        },
        {
          "id": "7271ec21-f996-4c31-b1cd-e1ac2d1932ea",
          "name": "removeTagsFromResource",
          "request": {
            "url": "http://example.com/api/?Action=RemoveTagsFromResource?ResourceARN=ResourceARN&TagKeys=TagKeys",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes one or more tags from the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7517b3c-57e6-4d45-afb9-1bf56c4af08d"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload Buffer",
      "item": [
        {
          "id": "609e7bf1-7d66-409e-b896-8c36376e1704",
          "name": "addUploadBuffer",
          "request": {
            "url": "http://example.com/api/?Action=AddUploadBuffer?DiskIds=DiskIds&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures one or more gateway local disks as upload buffer for a specified gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3b4219e-299a-4e07-b647-119a4cf2d117"
            }
          ]
        },
        {
          "id": "627f01fe-8c25-41f5-8487-0455a7ac0d78",
          "name": "describeUploadBuffer",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUploadBuffer?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the upload buffer of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15dba93e-1146-4ea9-8ff7-68aa2184b405"
            }
          ]
        }
      ]
    },
    {
      "name": "Working Storage",
      "item": [
        {
          "id": "b63e938b-5310-412e-a6b7-b80f2e2a2763",
          "name": "addWorkingStorage",
          "request": {
            "url": "http://example.com/api/?Action=AddWorkingStorage?DiskIds=DiskIds&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures one or more gateway local disks as working storage for a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e2b53a4-007d-448d-8a53-9d1b9ccaff56"
            }
          ]
        },
        {
          "id": "23078e7c-b754-4e35-be81-725b14411064",
          "name": "describeWorkingStorage",
          "request": {
            "url": "http://example.com/api/?Action=DescribeWorkingStorage?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the working storage of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29c6e9ab-fe02-454a-a176-f98f02574963"
            }
          ]
        }
      ]
    },
    {
      "name": "Archival",
      "item": [
        {
          "id": "7c8cb9fd-334d-4b2b-b41f-d01752981521",
          "name": "cancelArchival",
          "request": {
            "url": "http://example.com/api/?Action=CancelArchival?GatewayARN=GatewayARN&TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels archiving of a virtual tape to the virtual tape shelf (VTS) after the\n         archiving process is initiated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76043a5a-266f-444b-8da5-20c3759ba181"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieval",
      "item": [
        {
          "id": "b832a6db-59bd-45d7-b13a-4994281e42ab",
          "name": "cancelRetrieval",
          "request": {
            "url": "http://example.com/api/?Action=CancelRetrieval?GatewayARN=GatewayARN&TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels retrieval of a virtual tape from the virtual tape shelf (VTS) to a gateway\n         after the retrieval process is initiated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f95e5c8-cb53-4cfb-a389-fc9a7519daf1"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volume",
      "item": [
        {
          "id": "3bc65708-f70a-40af-ae32-71ef9f6aa74e",
          "name": "createCachediSCSIVolume",
          "request": {
            "url": "http://example.com/api/?Action=CreateCachediSCSIVolume?ClientToken=ClientToken&GatewayARN=GatewayARN&NetworkInterfaceId=NetworkInterfaceId&SnapshotId=SnapshotId&SourceVolumeARN=SourceVolumeARN&TargetName=TargetName&VolumeSizeInBytes=VolumeSizeInBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a cached volume on a specified cached gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04e04d09-1eda-44a0-a4dc-3f19138d9da5"
            }
          ]
        }
      ]
    },
    {
      "name": "NFS File Share",
      "item": [
        {
          "id": "cc7561f7-232f-449f-b864-9c8e31b86f31",
          "name": "createNFSFileShare",
          "request": {
            "url": "http://example.com/api/?Action=CreateNFSFileShare?ClientToken=ClientToken&DefaultStorageClass=DefaultStorageClass&GatewayARN=GatewayARN&KMSEncrypted=KMSEncrypted&KMSKey=KMSKey&LocationARN=LocationARN&NFSFileShareDefaults=NFSFileShareDefaults&Role=Role",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a file share on an existing file gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "367febb2-3d4d-4152-8c93-30f5488e6bc5"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "8826ca97-1b8e-4a72-bde2-fe7da9c69902",
          "name": "createSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshot?SnapshotDescription=SnapshotDescription&VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates a snapshot of a volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7099110-04a2-414e-9f7f-e0da26a91880"
            }
          ]
        },
        {
          "id": "bfd439e7-0957-4180-ab3b-d4c2bf082abe",
          "name": "createSnapshotFromVolumeRecoveryPoint",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshotFromVolumeRecoveryPoint?SnapshotDescription=SnapshotDescription&VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates a snapshot of a gateway from a volume recovery point."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23519b62-428f-4f35-ba1a-4a78dc16b257"
            }
          ]
        },
        {
          "id": "48dd2854-8ae6-4eb0-9ad2-9a049ee6a998",
          "name": "deleteSnapshotSchedule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSnapshotSchedule?VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a snapshot of a volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc80b117-bd8c-44dc-9c3c-7cd34649306b"
            }
          ]
        },
        {
          "id": "76dfce7a-26e7-4c74-9833-3b0596535ec8",
          "name": "describeSnapshotSchedule",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSnapshotSchedule?VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the snapshot schedule for the specified gateway volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0bc56f8-0a31-4498-b4c7-6133dd344a5b"
            }
          ]
        }
      ]
    },
    {
      "name": "Stored SCSI Volume",
      "item": [
        {
          "id": "d4d97f39-3c5c-4de3-afc8-5f6b3bd319f6",
          "name": "createStorediSCSIVolume",
          "request": {
            "url": "http://example.com/api/?Action=CreateStorediSCSIVolume?DiskId=DiskId&GatewayARN=GatewayARN&NetworkInterfaceId=NetworkInterfaceId&PreserveExistingData=PreserveExistingData&SnapshotId=SnapshotId&TargetName=TargetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a volume on a specified gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28ffc780-4fad-40fe-9a79-8f745cdd198e"
            }
          ]
        }
      ]
    },
    {
      "name": "Tapes",
      "item": [
        {
          "id": "c4184a67-3038-430e-bb93-2cf243f29fa8",
          "name": "createTapes",
          "request": {
            "url": "http://example.com/api/?Action=CreateTapes?ClientToken=ClientToken&GatewayARN=GatewayARN&NumTapesToCreate=NumTapesToCreate&TapeBarcodePrefix=TapeBarcodePrefix&TapeSizeInBytes=TapeSizeInBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates one or more virtual tapes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc14b8c0-33ba-4d3e-b7a7-9d86b709c74d"
            }
          ]
        },
        {
          "id": "49b2ff90-f93a-40a5-b604-11cf494ca1e9",
          "name": "deleteTape",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTape?GatewayARN=GatewayARN&TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified virtual tape."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86f17ecb-89ad-428a-b46c-55637cd344b3"
            }
          ]
        },
        {
          "id": "a4aef940-ed55-4898-bb48-9d90cc16e8b6",
          "name": "deleteTapeArchive",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTapeArchive?TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified virtual tape from the virtual tape shelf (VTS)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78d78c9f-667c-438d-b052-9d5923afebf5"
            }
          ]
        },
        {
          "id": "5f43e573-e57b-43de-95ec-bb5a96e7a63c",
          "name": "describeTapes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTapes?GatewayARN=GatewayARN&Limit=Limit&Marker=Marker&TapeARNs=TapeARNs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of the specified Amazon Resource Name (ARN) of virtual tapes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24b4571e-afa8-4359-8ca0-0967cc86f655"
            }
          ]
        },
        {
          "id": "49fcbfdf-ffb8-441a-a724-97e5c6f17536",
          "name": "listTapes",
          "request": {
            "url": "http://example.com/api/?Action=ListTapes?Limit=Limit&Marker=Marker&TapeARNs=TapeARNs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists virtual tapes in your virtual tape library (VTL) and your virtual tape shelf\n         (VTS)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fd082a4-e1e0-44cf-860e-62e1305535eb"
            }
          ]
        },
        {
          "id": "32d7a52e-7010-47d3-8ee2-872e6cfaba14",
          "name": "retrieveTapeArchive",
          "request": {
            "url": "http://example.com/api/?Action=RetrieveTapeArchive?GatewayARN=GatewayARN&TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves an archived virtual tape from the virtual tape shelf (VTS) to a\n         gateway-VTL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a88a66cc-66d2-4532-adf8-46cfa1fa8983"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape With Barcode",
      "item": [
        {
          "id": "df09938d-1788-4ceb-acbb-504d6e643e30",
          "name": "createTapeWithBarcode",
          "request": {
            "url": "http://example.com/api/?Action=CreateTapeWithBarcode?GatewayARN=GatewayARN&TapeBarcode=TapeBarcode&TapeSizeInBytes=TapeSizeInBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a virtual tape by using your own barcode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "180ad8ce-7b96-4bb3-947d-2cbd42d39c2a"
            }
          ]
        }
      ]
    },
    {
      "name": "Bandwidth Rate Limit",
      "item": [
        {
          "id": "3ec650ee-4333-415f-a03f-65a0fbbc9864",
          "name": "deleteBandwidthRateLimit",
          "request": {
            "url": "http://example.com/api/?Action=DeleteBandwidthRateLimit?BandwidthType=BandwidthType&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the bandwidth rate limits of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bcce140-5ac5-4be7-9dfc-dd10f3eb745b"
            }
          ]
        },
        {
          "id": "a0c836f3-3b4b-4de7-82e4-8c5db3a5e50a",
          "name": "describeBandwidthRateLimit",
          "request": {
            "url": "http://example.com/api/?Action=DescribeBandwidthRateLimit?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the bandwidth rate limits of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a844ff56-a4ef-4a60-9e53-eeb32ed1e422"
            }
          ]
        }
      ]
    },
    {
      "name": "Chap Credentials",
      "item": [
        {
          "id": "391be8fd-f5f8-46d8-833d-5dd43cf0049d",
          "name": "deleteChapCredentials",
          "request": {
            "url": "http://example.com/api/?Action=DeleteChapCredentials?InitiatorName=InitiatorName&TargetARN=TargetARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes Challenge-Handshake Authentication Protocol (CHAP) credentials for a\n         specified iSCSI target and initiator pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e14f936b-98b4-44b0-a5d2-196f0447c326"
            }
          ]
        },
        {
          "id": "3dfce45c-98e1-4bee-8a17-57885d830c4c",
          "name": "describeChapCredentials",
          "request": {
            "url": "http://example.com/api/?Action=DescribeChapCredentials?TargetARN=TargetARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an array of Challenge-Handshake Authentication Protocol (CHAP) credentials\n         information for a specified iSCSI target, one for each target-initiator pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "415b6c34-e7ea-4c66-99bf-f434828699c9"
            }
          ]
        }
      ]
    },
    {
      "name": "File Share",
      "item": [
        {
          "id": "241b9c99-9703-4a93-b3a9-442442d58eb9",
          "name": "deleteFileShare",
          "request": {
            "url": "http://example.com/api/?Action=DeleteFileShare?FileShareARN=FileShareARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a file share from a file gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2130b76f-092f-4ba5-a2a0-ed8ba70311fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Volumes",
      "item": [
        {
          "id": "02cb6552-1e41-4890-932e-16cd89e3ab97",
          "name": "deleteVolume",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVolume?VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified gateway volume that you previously created using the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5a16fcf-50ac-41f9-a6fe-7374d7c37fb7"
            }
          ]
        },
        {
          "id": "9008cfd8-8555-4ed4-8ffb-6fb34cf266cc",
          "name": "listVolumes",
          "request": {
            "url": "http://example.com/api/?Action=ListVolumes?GatewayARN=GatewayARN&Limit=Limit&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the iSCSI stored volumes of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53996c21-16f6-4aee-aae4-a809bb17db21"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volumes",
      "item": [
        {
          "id": "9ead5b30-f766-41fa-9eba-90cd3684fece",
          "name": "describeCachediSCSIVolumes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCachediSCSIVolumes?VolumeARNs=VolumeARNs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of the gateway volumes specified in the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4455ff6c-66f7-4cfd-b902-34bc46efe0cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "a2e31372-7bb9-4fc9-bcd0-3fd3ead4ee21",
          "name": "describeMaintenanceStartTime",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceStartTime?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns your gateway's weekly maintenance start time including the day and time of\n         the week."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe5334e7-1792-4d62-9cb6-bad0fc008384"
            }
          ]
        }
      ]
    },
    {
      "name": "NFS File Shares",
      "item": [
        {
          "id": "cf13a973-4765-4aa6-b77a-48646b014e45",
          "name": "describeNFSFileShares",
          "request": {
            "url": "http://example.com/api/?Action=DescribeNFSFileShares?FileShareARNList=FileShareARNList",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a description for one or more file shares from a file gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3c90361-81bb-446b-bf80-cf2d0e2a554b"
            }
          ]
        }
      ]
    },
    {
      "name": "Stored SCSI Volumes",
      "item": [
        {
          "id": "f1f3dd6a-0232-42ac-90e1-9ee2a0a6e1d6",
          "name": "describeStorediSCSIVolumes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStorediSCSIVolumes?VolumeARNs=VolumeARNs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the description of the gateway volumes specified in the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a484f6f-73e3-429b-b503-297855aa93c2"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape Archives",
      "item": [
        {
          "id": "d431e0dc-a559-4f78-be97-cd4a70d26329",
          "name": "describeTapeArchives",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTapeArchives?Limit=Limit&Marker=Marker&TapeARNs=TapeARNs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of specified virtual tapes in the virtual tape shelf\n         (VTS)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0806425-8f24-4e51-9148-1ca23d9d372a"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape Recovery Points",
      "item": [
        {
          "id": "86aa5142-f10d-4609-aef4-48121b924bbe",
          "name": "describeTapeRecoveryPoints",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTapeRecoveryPoints?GatewayARN=GatewayARN&Limit=Limit&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of virtual tape recovery points that are available for the specified\n         gateway-VTL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3adbb76-7ce9-4932-a611-dab9032584c5"
            }
          ]
        }
      ]
    },
    {
      "name": "VTL Devices",
      "item": [
        {
          "id": "4ab26fa9-9270-4d91-87e9-9b2cc3918763",
          "name": "describeVTLDevices",
          "request": {
            "url": "http://example.com/api/?Action=DescribeVTLDevices?GatewayARN=GatewayARN&Limit=Limit&Marker=Marker&VTLDeviceARNs=VTLDeviceARNs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of virtual tape library (VTL) devices for the specified\n         gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c40a731-624b-4a20-be4a-d02e8c29b8d1"
            }
          ]
        }
      ]
    },
    {
      "name": "File Shares",
      "item": [
        {
          "id": "d54ae794-be40-4c19-95e0-db951f9dace9",
          "name": "listFileShares",
          "request": {
            "url": "http://example.com/api/?Action=ListFileShares?GatewayARN=GatewayARN&Limit=Limit&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of the file shares for a specific file gateway, or the list of file shares that belong to the calling user account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbb2d495-f0c0-4397-8b5d-86f28b36885e"
            }
          ]
        }
      ]
    },
    {
      "name": "Gateways",
      "item": [
        {
          "id": "9336120e-81eb-42db-aa96-9ae253bc9be3",
          "name": "listGateways",
          "request": {
            "url": "http://example.com/api/?Action=ListGateways?Limit=Limit&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists gateways owned by an AWS account in a region specified in the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66341e50-bd68-4ee2-84a5-a27ddae19310"
            }
          ]
        }
      ]
    },
    {
      "name": "Local Disks",
      "item": [
        {
          "id": "f4607f4b-94b3-40c5-8c1d-f68d7d35d500",
          "name": "listLocalDisks",
          "request": {
            "url": "http://example.com/api/?Action=ListLocalDisks?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the gateway's local disks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ee7f6ac-8356-4f22-ab36-3bd01a09e517"
            }
          ]
        }
      ]
    },
    {
      "name": "Volume Initiators",
      "item": [
        {
          "id": "113b3d8f-d50c-4e91-a6f6-c4c881f5afe3",
          "name": "listVolumeInitiators",
          "request": {
            "url": "http://example.com/api/?Action=ListVolumeInitiators?VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists iSCSI initiators that are connected to a volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cefdc4ab-ef8e-4b5c-b891-4b368392dbeb"
            }
          ]
        }
      ]
    },
    {
      "name": "Volume Recovery",
      "item": [
        {
          "id": "76e25099-5dee-4fab-9f9e-9cfaccecb614",
          "name": "listVolumeRecoveryPoints",
          "request": {
            "url": "http://example.com/api/?Action=ListVolumeRecoveryPoints?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the recovery points for a specified gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d15fdca6-d01f-48a5-b757-3599d08e4e48"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape Recovery",
      "item": [
        {
          "id": "ce9936f7-4ee7-48d3-8b72-2f98ca823dac",
          "name": "retrieveTapeRecoveryPoint",
          "request": {
            "url": "http://example.com/api/?Action=RetrieveTapeRecoveryPoint?GatewayARN=GatewayARN&TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the recovery point for the specified virtual tape."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "963eaf9e-657f-4f01-a12a-8ab431e0f804"
            }
          ]
        }
      ]
    },
    {
      "name": "Local Console Password",
      "item": [
        {
          "id": "d03ead04-11e9-4104-af0b-08b2aa346083",
          "name": "setLocalConsolePassword",
          "request": {
            "url": "http://example.com/api/?Action=SetLocalConsolePassword?GatewayARN=GatewayARN&LocalConsolePassword=LocalConsolePassword",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the password for your VM local console."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "027e1c09-b9bf-4fc1-928d-1d308bdc13fb"
            }
          ]
        }
      ]
    }
  ]
}