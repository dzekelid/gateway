{
  "info": {
    "name": "AWS Storage Gateway Service API Delete Gateway",
    "_postman_id": "46ec1a92-9b65-45e5-821c-903d2fb721fa",
    "description": "Deletes a gateway.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gateway",
      "item": [
        {
          "id": "06f906d5-3739-4163-9a56-af48112ddfd5",
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
              "id": "0bfbddc1-98e0-4507-92d7-c1057895ba31"
            }
          ]
        },
        {
          "id": "e6da156d-fb82-4de3-b799-1a8939eb724f",
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
              "id": "b304fa9c-60e9-4e72-b293-846ebf52bc0a"
            }
          ]
        }
      ]
    },
    {
      "name": "Cache",
      "item": [
        {
          "id": "1a6eb645-f9b2-47be-957d-14c40804ebae",
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
              "id": "ee6b41a5-8279-48a0-b4bb-eae7064dd277"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "5865a5b2-49f0-4df7-8e95-337cf48cfd62",
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
              "id": "61551cf9-3bf6-404a-b8a4-e708df0db598"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload Buffer",
      "item": [
        {
          "id": "5b05e1df-1563-4965-853b-a711693038ee",
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
              "id": "0850659b-412c-4597-9e86-e3d876940dfd"
            }
          ]
        }
      ]
    },
    {
      "name": "Working Storage",
      "item": [
        {
          "id": "512156b3-7e95-403b-bdbb-c42561a418cb",
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
              "id": "cb45c37a-ba64-401d-9061-5a3ff0689647"
            }
          ]
        }
      ]
    },
    {
      "name": "Archival",
      "item": [
        {
          "id": "69b4f18a-7bc7-4e8e-bb8a-4478dff182e6",
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
              "id": "bacaac0f-848f-49e2-9692-77696da20506"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieval",
      "item": [
        {
          "id": "21b8d119-141c-41ec-87c0-4a7451f2ab7d",
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
              "id": "b25b7dc6-8386-47fa-9181-3da9d130c4f2"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volume",
      "item": [
        {
          "id": "9f62343e-7b5f-4514-9051-02635aa73ee6",
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
              "id": "5a7b7322-57f6-4752-8bca-f9e3aee87558"
            }
          ]
        }
      ]
    },
    {
      "name": "NFS File Share",
      "item": [
        {
          "id": "8c20d5b1-17af-48b5-80dc-d457317c3fa9",
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
              "id": "832e6ff9-a205-4a15-9e7a-9ef5148be8bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "d2b54d58-c3f0-42a2-8b14-f39f056a867c",
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
              "id": "44b67d5a-42ef-4d18-9b17-8c158429e3c6"
            }
          ]
        },
        {
          "id": "13abd5eb-c61d-45c0-b3d6-1e2536f9fe74",
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
              "id": "49dc2573-0534-4e56-8f52-9cd4dd6f91e8"
            }
          ]
        }
      ]
    },
    {
      "name": "Stored SCSI Volume",
      "item": [
        {
          "id": "05448e5f-456b-4f6a-9e59-9d07879465e3",
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
              "id": "19556540-dcb7-4ce4-ba6d-a37883582ef2"
            }
          ]
        }
      ]
    },
    {
      "name": "Tapes",
      "item": [
        {
          "id": "48bcab96-edd2-4279-ac31-60a35c98ea49",
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
              "id": "ee3905c7-8db8-43c3-b0e6-a482ffbf2968"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape With Barcode",
      "item": [
        {
          "id": "9224b94f-cba5-4aa3-ad8d-1a58bb1d3f7f",
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
              "id": "82defc4f-0c01-4546-b42d-3aaba44c0aed"
            }
          ]
        }
      ]
    },
    {
      "name": "Bandwidth Rate Limit",
      "item": [
        {
          "id": "e62bae3e-a4ba-4f67-b1ca-cf2c58d50b36",
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
              "id": "e018368e-6fe5-40f9-988a-771637f309a2"
            }
          ]
        }
      ]
    },
    {
      "name": "Chap Credentials",
      "item": [
        {
          "id": "46b83728-799f-4968-82fa-7e5cefa10b20",
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
              "id": "04a7331b-ca41-4fa0-8728-6e7ee411aac7"
            }
          ]
        }
      ]
    },
    {
      "name": "File Share",
      "item": [
        {
          "id": "db31a855-a7b1-4ab9-a088-5f710544a907",
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
              "id": "405cb602-e4b4-4ba2-b75d-2ab475622456"
            }
          ]
        }
      ]
    }
  ]
}