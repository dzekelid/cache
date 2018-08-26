{
  "info": {
    "name": "AWS Storage Gateway Service API Reset Cache",
    "_postman_id": "17ef4e62-2676-4176-b807-9aaa6268473f",
    "description": "Resets all cache disks that have encountered a error and makes the disks available\n         for reconfiguration as cache storage.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gateway",
      "item": [
        {
          "id": "25c756da-f314-4eb2-b093-f2f8bb29c995",
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
              "id": "2c3f1652-7339-4771-945b-0608a453eec6"
            }
          ]
        },
        {
          "id": "0100de05-2f12-42a9-a4e6-c08ec5ba19cc",
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
              "id": "ce9c1c0a-a608-495c-8bed-3c381568c3bd"
            }
          ]
        },
        {
          "id": "4308f0fd-bd45-4dce-8792-d5507f18c8c3",
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
              "id": "920ddb77-d335-4b2c-92e8-de5bcc4b0c73"
            }
          ]
        },
        {
          "id": "09118fe4-6cca-4acf-9306-bae51c69ef29",
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
              "id": "12968ea9-7cda-4ada-9437-a09a4bf33025"
            }
          ]
        }
      ]
    },
    {
      "name": "Cache",
      "item": [
        {
          "id": "4c66b13c-3e50-40b4-ac19-bf0981bd3e30",
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
              "id": "9a75129d-b27d-4e49-9e83-4ee3e889d56f"
            }
          ]
        },
        {
          "id": "2213965b-d1c1-4c50-98bb-3b4ef87a9c32",
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
              "id": "a75f3312-82f5-4217-a84c-d5e8a0095255"
            }
          ]
        },
        {
          "id": "addee6e4-9673-4efd-8310-49bed2fb8ef6",
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
              "id": "d8f5f341-e928-47af-b3d9-15d422e5ff39"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "05a793ab-6a62-4f9a-88f8-4c14842b1893",
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
              "id": "c7a43f91-322a-4976-9afd-b25c16387815"
            }
          ]
        },
        {
          "id": "927cfe3f-5d1f-48ce-8059-94be8ab23ef5",
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
              "id": "fcee68b7-4ade-476f-bad7-51c27e316d45"
            }
          ]
        },
        {
          "id": "0919b396-811e-4705-aeb2-4532f3769e0c",
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
              "id": "204d6e80-c06f-4e8f-b899-33e69ee8a60c"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload Buffer",
      "item": [
        {
          "id": "d48ffa13-3d4d-41d6-8cc7-13d3c41fa512",
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
              "id": "f0593f50-7814-44ac-8131-1b3a34d58fa8"
            }
          ]
        },
        {
          "id": "1ca82513-b097-4f81-afa7-39862804c09f",
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
              "id": "9655c770-d0cb-4f4f-9839-9497355ab1dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Working Storage",
      "item": [
        {
          "id": "6bfb83aa-2263-4245-bdc4-050ca8336e8c",
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
              "id": "d023a64f-da62-4859-b931-078337a5103b"
            }
          ]
        },
        {
          "id": "37b1fb03-d4fc-4547-8597-17641017f246",
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
              "id": "0690d62a-4dae-4256-a878-16013cb10a09"
            }
          ]
        }
      ]
    },
    {
      "name": "Archival",
      "item": [
        {
          "id": "9bd9fe7b-2814-4e80-a4b7-290e2e43bcd9",
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
              "id": "5a94fba7-0ce9-49b3-a8ca-49e82e0da0b4"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieval",
      "item": [
        {
          "id": "a1b6a7b6-3513-4311-88af-9af10268c1c4",
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
              "id": "2ba94ff7-d282-44e1-b15e-df1322fa9519"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volume",
      "item": [
        {
          "id": "f1d83592-8b31-40a9-9402-7719d6b60ca7",
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
              "id": "43928ee3-4f7c-4eb9-8004-cd43aa9fbbcf"
            }
          ]
        }
      ]
    },
    {
      "name": "NFS File Share",
      "item": [
        {
          "id": "9c42eeda-43b8-4a90-aecf-82fc0c5d00c9",
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
              "id": "fd1e3c57-8ee5-4481-b76b-23df98530d96"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "8f826aaa-8ea5-4fd8-b224-8fdc79bbd445",
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
              "id": "6cd55b35-413f-4428-acfa-6febcb8490d2"
            }
          ]
        },
        {
          "id": "55e878ad-b552-4684-b852-eaadca2fe65f",
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
              "id": "02d21d1f-5592-452f-859f-c927f94b9690"
            }
          ]
        },
        {
          "id": "d8a15958-24d7-46a0-88d1-f79900f21169",
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
              "id": "2efad5e8-8ae0-45e3-9da2-f2b065e84f18"
            }
          ]
        },
        {
          "id": "fb84cc31-7f70-41c6-8dc7-d966ccc89dd9",
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
              "id": "21465bf2-b0d5-4172-bf78-f8df3f2386a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Stored SCSI Volume",
      "item": [
        {
          "id": "f6681b99-02cf-4a94-925d-2fddcbbd1ada",
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
              "id": "5781d1c2-fd91-47dd-aabd-a7bb5921a90d"
            }
          ]
        }
      ]
    },
    {
      "name": "Tapes",
      "item": [
        {
          "id": "7bc8b624-a765-442c-9826-bbb2635ecfc6",
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
              "id": "4f037bea-99de-4033-9595-4eecbb409cd1"
            }
          ]
        },
        {
          "id": "2c30239e-bd64-4c08-8eba-7634877edbc2",
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
              "id": "c08f87da-6457-4816-9f2b-258076c78061"
            }
          ]
        },
        {
          "id": "f70c9390-edd0-4b4b-9b97-767001de79d3",
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
              "id": "20ed3082-d91e-4a89-952e-818d82111aa7"
            }
          ]
        },
        {
          "id": "65455de9-36bb-42dd-a154-7074514c946c",
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
              "id": "158fa1fd-beb1-499d-9cc6-60dfd5bf19f0"
            }
          ]
        },
        {
          "id": "c9eef4c6-94ff-4b48-bfeb-3a94c9d8f3d6",
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
              "id": "09bded76-7b99-4db7-b431-bd968cd4ecc4"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape With Barcode",
      "item": [
        {
          "id": "7a31f48a-e262-4304-b4bc-2add1bb2229d",
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
              "id": "79e4324e-8f19-4cea-bf16-95ff34fa7189"
            }
          ]
        }
      ]
    },
    {
      "name": "Bandwidth Rate Limit",
      "item": [
        {
          "id": "178ec626-b082-4c31-bebb-cea67ab0d87e",
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
              "id": "f1bd4a00-41af-4780-ac1e-6ecc0cc09e2d"
            }
          ]
        },
        {
          "id": "a8b6956e-97a9-402f-8f3c-5b18d4da066e",
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
              "id": "1b390290-5de3-48e0-959c-97708e55b691"
            }
          ]
        }
      ]
    },
    {
      "name": "Chap Credentials",
      "item": [
        {
          "id": "37ab9d3c-3d5e-4db8-b72e-5d5a18ba6e0e",
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
              "id": "0a4b00ff-1253-40c2-946c-3ce14107de83"
            }
          ]
        },
        {
          "id": "738f9b56-ef3e-4590-b800-eec56a7b7cb5",
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
              "id": "847b2ece-4f62-4aed-b99d-00c92fc97430"
            }
          ]
        }
      ]
    },
    {
      "name": "File Share",
      "item": [
        {
          "id": "24bd9e28-659a-4436-a014-cee73ee6ae3b",
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
              "id": "c20d18c1-b43f-4107-9783-e57859195bf0"
            }
          ]
        }
      ]
    },
    {
      "name": "Volumes",
      "item": [
        {
          "id": "f4ae07b2-9993-4fd7-9f56-e91177838de8",
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
              "id": "dedbadbc-3950-486a-859a-d0f6fdcbc86a"
            }
          ]
        },
        {
          "id": "00c181cd-9a8e-41da-9eee-6e3c4e280ea3",
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
              "id": "ee46b89d-8b45-415a-bb33-9dd68936bd32"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volumes",
      "item": [
        {
          "id": "48e28520-c64a-4a1b-ad98-c903d4e858c1",
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
              "id": "a1d102a1-9e1a-4659-a5b3-8af48057f043"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "5a2459fe-971d-461b-8146-c08345357234",
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
              "id": "fcd5ac26-d2a9-45d7-b26f-8db20f80a572"
            }
          ]
        }
      ]
    },
    {
      "name": "NFS File Shares",
      "item": [
        {
          "id": "7dda3107-0982-48d7-911b-2e04f89b56c7",
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
              "id": "773631ef-90fa-4541-98c4-c8ced34cf7bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Stored SCSI Volumes",
      "item": [
        {
          "id": "0a6b810c-36d1-48c7-85b9-3ef8c0355503",
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
              "id": "28b6b289-cece-4383-b305-7dbd08cf9173"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape Archives",
      "item": [
        {
          "id": "53e040e3-aacf-4e41-aeff-e4c6785c4015",
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
              "id": "0ba3d6b0-6a94-4c05-943d-9d0016982698"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape Recovery Points",
      "item": [
        {
          "id": "673e23e5-1a3e-4061-9fee-fa5bc9fa1542",
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
              "id": "b8531ea6-8ffc-4434-812a-fe5c7a24db54"
            }
          ]
        }
      ]
    },
    {
      "name": "VTL Devices",
      "item": [
        {
          "id": "ea7f900d-41e7-45c1-b6cb-4921519e78da",
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
              "id": "99527ca5-4525-4ab0-abb8-fddf7b12f3ff"
            }
          ]
        }
      ]
    },
    {
      "name": "File Shares",
      "item": [
        {
          "id": "5463fc26-c00b-4fb5-96dc-1e186fcdc629",
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
              "id": "234bc683-6541-46f2-b4ea-8b910fcd16f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Gateways",
      "item": [
        {
          "id": "34c2af4d-e0ae-4ab0-9a66-16462ca35a36",
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
              "id": "1117d2b6-7974-4ebc-a8a5-cea5e626e46a"
            }
          ]
        }
      ]
    },
    {
      "name": "Local Disks",
      "item": [
        {
          "id": "acf3aa1b-ebed-4cd7-820c-6e6309ff3bb9",
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
              "id": "3e3ec50b-05b8-42cc-abb5-ab3ed913ee1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Volume Initiators",
      "item": [
        {
          "id": "f5d63e40-ffa5-425e-bea4-f8cccd10f4d0",
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
              "id": "84448c17-2b03-47ac-a5f1-3bb44e5218f2"
            }
          ]
        }
      ]
    },
    {
      "name": "Volume Recovery",
      "item": [
        {
          "id": "6f0cca78-eb94-458c-8d0b-640735e601ee",
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
              "id": "23df28f0-6b72-459f-af9b-ad52ccfec00a"
            }
          ]
        }
      ]
    }
  ]
}