{
  "info": {
    "name": "AWS Storage Gateway Service API Create Cached SCSI Volume",
    "_postman_id": "5508a553-bb78-4292-a52a-6d3dade3611a",
    "description": "Creates a cached volume on a specified cached gateway.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gateway",
      "item": [
        {
          "id": "6045e416-8267-4ec2-9f25-58ff14bcf828",
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
              "id": "54f1dfd7-58d0-4dc8-a542-49f61c8fddb3"
            }
          ]
        }
      ]
    },
    {
      "name": "Cache",
      "item": [
        {
          "id": "ae01bd38-d082-4f7e-8811-4d85e3f92bac",
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
              "id": "e2199d23-9823-46b5-9d19-e2a84eefd239"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "4dad09c9-b849-475d-a167-dbb7e75397af",
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
              "id": "c5a127a5-dbb6-486f-9e0e-bdd6a4923df7"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload Buffer",
      "item": [
        {
          "id": "dfd85432-90d8-4a1f-b571-fa05e8dafca4",
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
              "id": "07d1d071-9842-4094-a85e-b3c8861ff0b7"
            }
          ]
        }
      ]
    },
    {
      "name": "Working Storage",
      "item": [
        {
          "id": "50d4aa16-5b11-41c6-b65a-167638b3c247",
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
              "id": "7d2d02c6-6a5d-442c-8dd5-927ebbfb8de7"
            }
          ]
        }
      ]
    },
    {
      "name": "Archival",
      "item": [
        {
          "id": "c7744279-8ee0-4bbd-8a56-6e973e74d181",
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
              "id": "5bf339f8-fe74-4865-903c-0e5f9463613a"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieval",
      "item": [
        {
          "id": "cf84353a-76e7-4e2a-9b07-a4abc04f48a1",
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
              "id": "a1dbe806-3ef0-457d-8ca4-811c4fe1898b"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volume",
      "item": [
        {
          "id": "4cd74990-ca13-4c7a-86e0-2dc12b64b361",
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
              "id": "f60b4bc7-8521-4232-af67-bc1c455a313d"
            }
          ]
        }
      ]
    }
  ]
}