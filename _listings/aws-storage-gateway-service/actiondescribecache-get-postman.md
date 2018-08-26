{
  "info": {
    "name": "AWS Storage Gateway Service API Describe Cache",
    "_postman_id": "c2acc635-bc58-45c9-b1c6-0668700edbfb",
    "description": "Returns information about the cache of a gateway.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gateway",
      "item": [
        {
          "id": "a8985c4f-d48a-4a96-af03-f83fd725cb40",
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
              "id": "3d589e78-bc0f-40a1-8062-7c8870e6652f"
            }
          ]
        },
        {
          "id": "d70646df-78f8-4894-9692-a18ce75d665f",
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
              "id": "7312d68e-59aa-469d-829a-c933e1bef0d2"
            }
          ]
        }
      ]
    },
    {
      "name": "Cache",
      "item": [
        {
          "id": "144deeae-5799-4cf4-9c0f-c3ca85469a59",
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
              "id": "6143834f-37eb-49cf-a647-16f6ae50bce5"
            }
          ]
        },
        {
          "id": "d6de60bc-129c-42c7-86e6-027449ed25cc",
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
              "id": "dbdcbebb-c334-4bed-9eef-1bb101ea21d2"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "9a02b2dd-c64a-42e9-8108-e8a09b202d9f",
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
              "id": "fb1ad1fa-e4b7-4a4b-97dd-e092a4eb89bb"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload Buffer",
      "item": [
        {
          "id": "aa01fa20-4dba-44c1-a3a2-ef0f5ad63518",
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
              "id": "409e413c-63d3-472c-a072-635ce24eab4e"
            }
          ]
        }
      ]
    },
    {
      "name": "Working Storage",
      "item": [
        {
          "id": "fc6c4b3b-72b4-48ef-8251-d6df5ab17634",
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
              "id": "f87b116f-9464-4da0-bf57-b90d52242bed"
            }
          ]
        }
      ]
    },
    {
      "name": "Archival",
      "item": [
        {
          "id": "d4d5f467-8444-4a42-9701-175ad366582c",
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
              "id": "deeb0c30-4425-4cba-a845-b3239e92c7c5"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieval",
      "item": [
        {
          "id": "83921657-ce15-4f73-a93e-e146d6c95b8f",
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
              "id": "e9215ee5-e28e-4aa4-baef-ac34baf4eaed"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volume",
      "item": [
        {
          "id": "0fd40d57-a335-476b-85cd-aa749d449562",
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
              "id": "98206a8c-b8bc-42af-866a-2111372ad8d3"
            }
          ]
        }
      ]
    },
    {
      "name": "NFS File Share",
      "item": [
        {
          "id": "2b462924-30c4-4c9f-8b46-f39ba3885b25",
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
              "id": "3a6f8019-0b9b-48db-950c-2d41384f7e90"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "17ef9a64-8925-4008-a63e-1cdb6414a238",
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
              "id": "f4637c51-a433-4bb5-af10-f9365d2d6099"
            }
          ]
        },
        {
          "id": "86936784-d82e-4efb-bea6-70e4491ae05c",
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
              "id": "b25aca76-349f-4bcd-b63e-da5692394a9c"
            }
          ]
        },
        {
          "id": "dd35d05b-9e3e-4777-9a48-24a613fffc7a",
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
              "id": "0147bb35-6f45-4b06-ac30-b6e31de2bc9d"
            }
          ]
        }
      ]
    },
    {
      "name": "Stored SCSI Volume",
      "item": [
        {
          "id": "7bbb0e28-4dcf-4df2-8dc0-a996fde85c38",
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
              "id": "3e86cb7f-9c84-4dbc-94a3-6a35b12aebc9"
            }
          ]
        }
      ]
    },
    {
      "name": "Tapes",
      "item": [
        {
          "id": "bd576b2a-1905-4636-b67e-e823fe73689c",
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
              "id": "4195e6f8-b9b3-42ea-b2ff-a461ed2fde1d"
            }
          ]
        },
        {
          "id": "9547eee0-2327-4709-a03b-54e4072537cc",
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
              "id": "0aa1cc4a-34b0-4206-8cbc-2416f001e0e9"
            }
          ]
        },
        {
          "id": "4823246a-76da-4d79-b810-282e44d1aa2e",
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
              "id": "073aaac7-03cd-472c-ba4f-d1e9b347e9eb"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape With Barcode",
      "item": [
        {
          "id": "30d5f04b-995a-4135-b01b-7cb0ef9fa8b3",
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
              "id": "1b77cd92-096b-40f1-bacb-31a94dc00921"
            }
          ]
        }
      ]
    },
    {
      "name": "Bandwidth Rate Limit",
      "item": [
        {
          "id": "72f3c52d-605b-4ce3-987c-8c6962aa7fd9",
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
              "id": "4cf2f88d-30be-4db6-bbaf-30fde9946c5a"
            }
          ]
        },
        {
          "id": "3d49c78d-d7fd-4bf2-b919-113a0f630503",
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
              "id": "7fa35e10-3518-4a42-982a-d1dfd87d830e"
            }
          ]
        }
      ]
    },
    {
      "name": "Chap Credentials",
      "item": [
        {
          "id": "941f706a-c9db-4552-a8fb-22f113c9fc09",
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
              "id": "f72bc52d-5d80-4b0b-a328-3435c18d257f"
            }
          ]
        }
      ]
    },
    {
      "name": "File Share",
      "item": [
        {
          "id": "6ca87c5b-33f8-4993-ad73-6489299c3ae3",
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
              "id": "2d8043cd-a946-472b-83e5-283d48e74d8b"
            }
          ]
        }
      ]
    },
    {
      "name": "Volumes",
      "item": [
        {
          "id": "66ffc892-9261-4538-ba50-17cce2d72b46",
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
              "id": "42425193-2c43-43bd-a1fb-e838d1b02b30"
            }
          ]
        }
      ]
    }
  ]
}