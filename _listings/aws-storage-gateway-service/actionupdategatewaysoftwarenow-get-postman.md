{
  "info": {
    "name": "AWS Storage Gateway Service API Update Gateway Software Now",
    "_postman_id": "bb3157b9-15b1-48d0-b913-40cd13a39eda",
    "description": "Updates the gateway virtual machine (VM) software.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gateway",
      "item": [
        {
          "id": "b6cfed4d-1463-4746-ae5f-79023c193831",
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
              "id": "69397f8f-9f5c-45dd-a5ee-978cd51fd9ea"
            }
          ]
        },
        {
          "id": "f026de6e-875c-4f8b-b753-bf972fc44bf1",
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
              "id": "0bcf2431-c2fb-4fbd-8408-57f68cef75ef"
            }
          ]
        },
        {
          "id": "11796db8-02d4-45a3-9a92-3ef8df75eb8f",
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
              "id": "fa8fa4b3-6bb6-49b4-9174-7b9c1a1b6c61"
            }
          ]
        },
        {
          "id": "8dbe7b17-4c15-4d4b-bda6-07ed762610f7",
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
              "id": "eb84be0b-08f0-4dd9-9049-d2e561118d00"
            }
          ]
        },
        {
          "id": "52a6570d-16e7-4a68-b636-b42608d512c6",
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
              "id": "76625b12-9ca2-4a84-93a7-9232474b5e12"
            }
          ]
        },
        {
          "id": "751f2b24-935d-4884-aea6-f3086b48a7dc",
          "name": "startGateway",
          "request": {
            "url": "http://example.com/api/?Action=StartGateway?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts a gateway that you previously shut down (see."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18f8b364-8a1c-4c0e-a9c8-a4c2b22f1f4f"
            }
          ]
        },
        {
          "id": "aa6ec6d4-ed24-4bd9-84d6-70dab0bb45a6",
          "name": "updateGatewayInformation",
          "request": {
            "url": "http://example.com/api/?Action=UpdateGatewayInformation?GatewayARN=GatewayARN&GatewayName=GatewayName&GatewayTimezone=GatewayTimezone",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a gateway's metadata, which includes the gateway's name and time zone."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f1f966b-259e-4a8d-888f-e2258bbd3e70"
            }
          ]
        },
        {
          "id": "deeedf55-5310-457e-828c-87daffda1d6d",
          "name": "updateGatewaySoftwareNow",
          "request": {
            "url": "http://example.com/api/?Action=UpdateGatewaySoftwareNow?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the gateway virtual machine (VM) software."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b5ad494-6deb-4479-bf30-2b3f2e0ab963"
            }
          ]
        }
      ]
    },
    {
      "name": "Cache",
      "item": [
        {
          "id": "61f9e99c-ede5-4baf-8833-ad39b574ebb6",
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
              "id": "5e4924ff-34b2-4e08-8850-e51535425b7f"
            }
          ]
        },
        {
          "id": "e7b3d97a-ca4c-4e8b-bba2-5c724f741999",
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
              "id": "14c7baf1-3f3e-4572-8568-7712d6be4576"
            }
          ]
        },
        {
          "id": "de42eaa2-4797-4585-a47b-6e21fcd0afe3",
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
              "id": "69920d16-cdd5-4352-b2dd-f844c66440a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "feb0a5ed-17f8-42c0-b225-433c6217ff7a",
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
              "id": "1cd86107-d168-4a68-a247-94a63fe3f054"
            }
          ]
        },
        {
          "id": "e788d2e5-3d04-478e-807e-685636676ee7",
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
              "id": "95b33c34-77f5-4fcc-a933-1921f808e2bf"
            }
          ]
        },
        {
          "id": "3685ebfa-5a84-4c63-8629-d1fcb10eb1ae",
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
              "id": "6ca8d101-080a-43fa-ad93-81922f856f66"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload Buffer",
      "item": [
        {
          "id": "717f3d52-d65e-4fad-8917-414dc5754104",
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
              "id": "e20b5559-8349-4158-a66f-92e19175c578"
            }
          ]
        },
        {
          "id": "a6467648-5fe4-4e1e-a529-656b0e2ffb06",
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
              "id": "c04eb71f-bce0-4e64-a92c-431d38fbcd74"
            }
          ]
        }
      ]
    },
    {
      "name": "Working Storage",
      "item": [
        {
          "id": "7cf0f5f7-2bb7-401a-a6c7-897438d66152",
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
              "id": "ef569a5c-0ccb-4ef6-b5a5-ac8cca0a4031"
            }
          ]
        },
        {
          "id": "4de64f1b-15e5-4e92-9a08-aa2d92617340",
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
              "id": "ac9bf056-55a4-4ac7-b570-f055e224b27d"
            }
          ]
        }
      ]
    },
    {
      "name": "Archival",
      "item": [
        {
          "id": "10e5ee1e-215b-4e7e-8446-dd4d3ad84120",
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
              "id": "d0582b17-f336-4e94-b340-a1bd3d3e2649"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieval",
      "item": [
        {
          "id": "5eca31ab-ad14-4c0d-b2ca-8fbfcb81c271",
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
              "id": "f975f07c-104a-40d2-8178-93039eee9e6d"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volume",
      "item": [
        {
          "id": "2c1dbbe9-ff42-476d-a368-75e5b48fab38",
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
              "id": "6a0287f4-eede-48ea-8f75-a46b45eefa7d"
            }
          ]
        }
      ]
    },
    {
      "name": "NFS File Share",
      "item": [
        {
          "id": "77727a42-1eec-4f19-9194-66bf48689465",
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
              "id": "ac87d0da-81ed-421e-aa94-356665d58930"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "d4e9203c-2ac0-40c6-8995-1b01f58bb608",
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
              "id": "93a74485-7d3c-4554-8796-dc97f04a8fb5"
            }
          ]
        },
        {
          "id": "35b61b17-19ee-4f47-921f-984bb7bb93c9",
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
              "id": "7f79c75d-04ce-4c78-9e49-13b25f0187d0"
            }
          ]
        },
        {
          "id": "56eeb69b-7a82-471a-bd63-c9fd5b59101e",
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
              "id": "a0497129-116b-455b-a533-1e78800d2305"
            }
          ]
        },
        {
          "id": "f964a211-2ccd-4cbf-a7ec-daea98c1b80e",
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
              "id": "80313780-892b-492c-b869-af01db681af4"
            }
          ]
        }
      ]
    },
    {
      "name": "Stored SCSI Volume",
      "item": [
        {
          "id": "a5d469dc-3e4c-4214-9707-796d5e078218",
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
              "id": "dcf01d07-bdd2-4d8c-b602-5a96c3c599ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Tapes",
      "item": [
        {
          "id": "6eaabcf8-9573-4625-9e45-413b4488ce43",
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
              "id": "2355cfca-2920-4ed4-9e6b-ef12c08f6c56"
            }
          ]
        },
        {
          "id": "b6d7c197-53e2-4066-896d-99905d8bd91f",
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
              "id": "cdd7a440-4d70-43e1-9920-c7f642988d86"
            }
          ]
        },
        {
          "id": "67b528f0-2caa-4000-9b38-d2928fa03463",
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
              "id": "9a1c35cf-a786-41c4-8112-f6c09dfbd876"
            }
          ]
        },
        {
          "id": "919fb4f1-bd5b-46d2-bb20-b414222fbcab",
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
              "id": "bb111728-66e6-4979-a485-4349438e48b7"
            }
          ]
        },
        {
          "id": "4f5df1cc-6890-4b1f-aa52-ab6f660bec90",
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
              "id": "0857bff4-aedf-4f7d-aa34-d729d754c834"
            }
          ]
        },
        {
          "id": "fa0fbe82-7017-4717-ab02-efa9fc49b09e",
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
              "id": "6ae39c69-af34-4cb7-af1f-10d46df3e82b"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape With Barcode",
      "item": [
        {
          "id": "87de2332-d1b5-4a95-bf18-eb0e91360f0d",
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
              "id": "087463e9-db2c-405d-ac27-fc8740adc312"
            }
          ]
        }
      ]
    },
    {
      "name": "Bandwidth Rate Limit",
      "item": [
        {
          "id": "8f8eb54e-123d-4b89-b4b1-e1dfe7af5ddf",
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
              "id": "6c835a5a-77c5-492a-b42c-f5a12b662f56"
            }
          ]
        },
        {
          "id": "905f2479-43cd-417c-b2de-d4a14ab25695",
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
              "id": "23ce417e-6a13-451b-b7b8-ae1a8c48ecde"
            }
          ]
        },
        {
          "id": "3b98e117-b9d4-4e62-9879-d269dd0167b5",
          "name": "updateBandwidthRateLimit",
          "request": {
            "url": "http://example.com/api/?Action=UpdateBandwidthRateLimit?AverageDownloadRateLimitInBitsPerSec=AverageDownloadRateLimitInBitsPerSec&AverageUploadRateLimitInBitsPerSec=AverageUploadRateLimitInBitsPerSec&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the bandwidth rate limits of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d37fbc9-218f-4cbc-9691-c1ec4ddcd8f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Chap Credentials",
      "item": [
        {
          "id": "1121395d-b098-4c58-b4e3-46da7edf43b4",
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
              "id": "14103272-dd92-4131-9011-60c28fdaa07a"
            }
          ]
        },
        {
          "id": "a92946c1-51dd-4c85-ac3d-16a5600113f4",
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
              "id": "f875e865-2158-484b-8e6b-ec8eebc0e5a3"
            }
          ]
        },
        {
          "id": "f20e2cb5-08b4-464b-b260-5d13dc151643",
          "name": "updateChapCredentials",
          "request": {
            "url": "http://example.com/api/?Action=UpdateChapCredentials?InitiatorName=InitiatorName&SecretToAuthenticateInitiator=SecretToAuthenticateInitiator&SecretToAuthenticateTarget=SecretToAuthenticateTarget&TargetARN=TargetARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the Challenge-Handshake Authentication Protocol (CHAP) credentials for a\n         specified iSCSI target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0af80379-fb05-4474-b071-98a679893b7a"
            }
          ]
        }
      ]
    },
    {
      "name": "File Share",
      "item": [
        {
          "id": "a73ee58d-f93d-4a7b-876b-8e96af6a368d",
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
              "id": "bcbeefd3-e57b-425f-a951-01dc6a40cdbd"
            }
          ]
        }
      ]
    },
    {
      "name": "Volumes",
      "item": [
        {
          "id": "c0f43274-c728-4ffb-9833-a09deba644ab",
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
              "id": "7b7edd07-35c7-4ae4-8981-500dc3400d75"
            }
          ]
        },
        {
          "id": "8094bf46-008a-4ce1-b580-ab9402bf6a35",
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
              "id": "55f2ffc6-288c-4c4d-9096-b17b767c281e"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volumes",
      "item": [
        {
          "id": "e53cec54-aba4-4ed0-8dae-2ea6f3fa0480",
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
              "id": "77eae840-05df-4af4-9edd-e26c48dcc0ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "a1d78b98-fabf-4426-8f4f-5b8fe4f346e0",
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
              "id": "27c5b2e5-6467-4adc-b590-64136aa7fdd0"
            }
          ]
        }
      ]
    },
    {
      "name": "NFS File Shares",
      "item": [
        {
          "id": "7c098c67-99f9-4130-9a34-969a84ce1663",
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
              "id": "42c640d6-bfba-4db4-bb8a-99a010ffd933"
            }
          ]
        }
      ]
    },
    {
      "name": "Stored SCSI Volumes",
      "item": [
        {
          "id": "73d79bbc-bd75-4e18-88ce-c26a515a336a",
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
              "id": "17311c8d-7cb2-4de4-b051-78dc472eccb2"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape Archives",
      "item": [
        {
          "id": "fa80618f-ba99-41f4-80dc-f8abc0466bf6",
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
              "id": "a75be385-e21a-4a86-9524-a226ebe9bd7e"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape Recovery Points",
      "item": [
        {
          "id": "435475b7-4f7b-4382-abc8-f13e05e68a72",
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
              "id": "5091a888-f754-49a0-8356-2c258c4ef967"
            }
          ]
        }
      ]
    },
    {
      "name": "VTL Devices",
      "item": [
        {
          "id": "9b808c7b-346e-45ab-ad23-b8cd57be8a17",
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
              "id": "1ba9e56d-65e3-4b06-b24c-39e169fd0ee7"
            }
          ]
        }
      ]
    },
    {
      "name": "File Shares",
      "item": [
        {
          "id": "ec498c13-8c85-49a0-87b0-90bde1c5cbe9",
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
              "id": "c4058db2-1969-4bb0-97a9-6e9e364205d7"
            }
          ]
        }
      ]
    },
    {
      "name": "Gateways",
      "item": [
        {
          "id": "a7b69e6e-a5f0-4118-b6f3-6d299f2f5760",
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
              "id": "c1132a32-d976-4aae-ba36-437c8ff2b5f5"
            }
          ]
        }
      ]
    },
    {
      "name": "Local Disks",
      "item": [
        {
          "id": "0707f46d-e138-42b4-8bb6-dcc7113917b3",
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
              "id": "c38899a1-5cdb-4fae-947b-619a8e2a7c22"
            }
          ]
        }
      ]
    },
    {
      "name": "Volume Initiators",
      "item": [
        {
          "id": "b9ed83de-a4b1-4e81-b440-7d1d2171cfe7",
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
              "id": "873212b2-54d0-4c12-a50c-56db4b6adbb9"
            }
          ]
        }
      ]
    },
    {
      "name": "Volume Recovery",
      "item": [
        {
          "id": "40c89086-39a2-41f1-ab81-a5c32ccb77a6",
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
              "id": "3f9476e4-297f-4b36-a876-cb419af18519"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape Recovery",
      "item": [
        {
          "id": "7ddce214-3621-4095-a66c-7043e2a43b00",
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
              "id": "59b1c9c2-b5be-4d94-be3d-fd8ce8ef04a9"
            }
          ]
        }
      ]
    },
    {
      "name": "Local Console Password",
      "item": [
        {
          "id": "8bc764c0-7276-4312-879b-116edd4c4940",
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
              "id": "0ea60dd8-c5fb-40b2-94ee-d62834c1e042"
            }
          ]
        }
      ]
    }
  ]
}