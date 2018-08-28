{
  "info": {
    "name": "AWS Device Farm API Update Device Pool",
    "_postman_id": "adf1fd2a-0b5d-4f22-930b-94aed65e1674",
    "description": "Modifies the name, description, and rules in a device pool given the attributes and the pool ARN.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device Pool",
      "item": [
        {
          "id": "e5110c22-ea5b-4244-9b45-c59c65b1fa0b",
          "name": "createDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=CreateDevicePool?description=description&name=name&projectArn=projectArn&rules=rules",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "072b47a3-3d96-4eaa-8f47-8e48919f2e38"
            }
          ]
        },
        {
          "id": "9879276f-4763-4757-b1b8-c81fafac5424",
          "name": "deleteDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a device pool given the pool ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47c78c29-afff-478d-9082-406bc60def60"
            }
          ]
        },
        {
          "id": "c670375f-0fb9-485e-9b19-876aac24d082",
          "name": "getDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a399f1d-d347-4d4a-b246-11d1286e6ee0"
            }
          ]
        },
        {
          "id": "0cd4d194-95c0-41a0-b10e-2ab9683f9e81",
          "name": "getDevicePoolCompatibility",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePoolCompatibility?appArn=appArn&devicePoolArn=devicePoolArn&testType=testType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about compatibility with a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "341f4d1e-ac0f-4ea1-b03b-50221e5b94bc"
            }
          ]
        },
        {
          "id": "b85acebd-83eb-4339-906b-2b158b704ff2",
          "name": "listDevicePools",
          "request": {
            "url": "http://example.com/api/?Action=ListDevicePools?arn=arn&nextToken=nextToken&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about device pools."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f363f543-112e-4306-8c38-1f28489419d2"
            }
          ]
        },
        {
          "id": "31ffa15f-857e-4517-8d24-fe7ad4a06a53",
          "name": "updateDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=UpdateDevicePool?arn=arn&description=description&name=name&rules=rules",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the name, description, and rules in a device pool given the attributes and the pool ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "631406fa-5201-44d2-8c1a-843affdec68d"
            }
          ]
        }
      ]
    },
    {
      "name": "Project",
      "item": [
        {
          "id": "017b5b94-14d8-4d3e-9249-8afda0effa69",
          "name": "createProject",
          "request": {
            "url": "http://example.com/api/?Action=CreateProject?name=name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89f7708a-2109-4205-8104-d46d29429afa"
            }
          ]
        }
      ]
    },
    {
      "name": "Remote Access Sessions",
      "item": [
        {
          "id": "a0156246-8cf6-45e5-a786-02af19d6e67c",
          "name": "createRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=CreateRemoteAccessSession?configuration=configuration&deviceArn=deviceArn&name=name&projectArn=projectArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specifies and starts a remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc193064-516a-4a34-9a9f-434e30b9d61a"
            }
          ]
        },
        {
          "id": "02ce75c3-1211-4eea-a4da-bdee56618a38",
          "name": "deleteRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a completed remote access session and its results."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "480467ce-2693-4945-994b-f00cbe561c2a"
            }
          ]
        },
        {
          "id": "b328fd69-62e4-4d55-96b8-4e7a748d1c3d",
          "name": "getRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=GetRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a link to a currently running remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d533bec-9e38-4ab9-9408-f630db95b045"
            }
          ]
        },
        {
          "id": "ae42a389-802a-41f0-aea5-8665a794cc56",
          "name": "installToRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=InstallToRemoteAccessSession?appArn=appArn&remoteAccessSessionArn=remoteAccessSessionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Installs an application to the device in a remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5427548a-c13c-4829-99ab-180b9b4ea3b5"
            }
          ]
        },
        {
          "id": "4fb1356f-2ce7-4135-8de0-b834a7a952c2",
          "name": "listRemoteAccessSessions",
          "request": {
            "url": "http://example.com/api/?Action=ListRemoteAccessSessions?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all currently running remote access sessions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38b34d87-c81b-4fab-ba72-b2f419e08ddf"
            }
          ]
        },
        {
          "id": "8bc67bee-3183-411b-aece-533795824f93",
          "name": "stopRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=StopRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Ends a specified remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f5f6e0f-6021-488b-ba84-3e14d1c7187f"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "d98507b8-074e-4f27-a8a2-eca9fbc295bd",
          "name": "createUpload",
          "request": {
            "url": "http://example.com/api/?Action=CreateUpload?contentType=contentType&name=name&projectArn=projectArn&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Uploads an app or test scripts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "994cbad1-b786-4899-942d-d0be415e6153"
            }
          ]
        },
        {
          "id": "60ff0713-12ef-4b5e-90b5-8e9295a5bca9",
          "name": "getUpload",
          "request": {
            "url": "http://example.com/api/?Action=GetUpload?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about an upload."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e372b8e-e89d-4272-a26d-8f8a93362627"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "05e0d6af-c997-4bcd-8751-3197aa84a824",
          "name": "deleteProject",
          "request": {
            "url": "http://example.com/api/?Action=DeleteProject?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Device Farm project, given the project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abd09477-ba44-45ef-bf10-50619fba03de"
            }
          ]
        },
        {
          "id": "51a69a89-cbf6-41d7-a123-f2601af17f5d",
          "name": "getProject",
          "request": {
            "url": "http://example.com/api/?Action=GetProject?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "105e5681-986d-466e-b459-2c551b13433b"
            }
          ]
        },
        {
          "id": "3d2b8a30-e476-4736-81e0-8b951f8558c4",
          "name": "listProjects",
          "request": {
            "url": "http://example.com/api/?Action=ListProjects?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about projects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "547a1431-b182-4868-acca-3933dcffabb1"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "dba05005-6587-4cf6-a28d-49e5d0526e00",
          "name": "deleteRun",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the run, given the run ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4e4203e-9417-47fd-8807-55c0fe8f9397"
            }
          ]
        },
        {
          "id": "2dedb0cf-3b9b-4f4f-bfeb-c44105b933dc",
          "name": "getRun",
          "request": {
            "url": "http://example.com/api/?Action=GetRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfedc4c8-2a49-496f-a848-36944ab54815"
            }
          ]
        },
        {
          "id": "038c0e87-6543-429e-bbcf-e00a9d37dacf",
          "name": "listRuns",
          "request": {
            "url": "http://example.com/api/?Action=ListRuns?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about runs, given an AWS Device Farm project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc059447-7d2e-43b9-94b2-2c98cbba30fb"
            }
          ]
        },
        {
          "id": "6268515b-d8aa-4bbf-aa21-2bb01cacdba0",
          "name": "scheduleRun",
          "request": {
            "url": "http://example.com/api/?Action=ScheduleRun?appArn=appArn&configuration=configuration&devicePoolArn=devicePoolArn&name=name&projectArn=projectArn&test=test",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Schedules a run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd003f37-6631-4b37-997e-9d128160ce48"
            }
          ]
        },
        {
          "id": "3733db0a-15a2-4e30-b3d4-9e2df1097c2c",
          "name": "stopRun",
          "request": {
            "url": "http://example.com/api/?Action=StopRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates a stop request for the current test run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd0c6ab9-635c-40ef-a5ec-edb297abe252"
            }
          ]
        }
      ]
    },
    {
      "name": "Uploads",
      "item": [
        {
          "id": "b0200164-0d42-4a05-8c3c-cad32e786f44",
          "name": "deleteUpload",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUpload?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an upload given the upload ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2283349-fd70-48f8-ad1d-58a8cef7c719"
            }
          ]
        },
        {
          "id": "7e37171c-2500-4055-894a-1021efe46ddb",
          "name": "listUploads",
          "request": {
            "url": "http://example.com/api/?Action=ListUploads?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about uploads, given an AWS Device Farm project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f14751b3-cb5b-48f3-9023-b95814ee4d78"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Settings",
      "item": [
        {
          "id": "20900bef-95d9-44fb-9eba-7e958b7c1721",
          "name": "getAccountSettings",
          "request": {
            "url": "http://example.com/api/?Action=GetAccountSettings?accountSettings=accountSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of unmetered iOS and/or unmetered Android devices that have been purchased by the account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "341f682a-b698-4b80-a809-82e61d132b74"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "9995b77c-39a2-495d-b486-34827c292240",
          "name": "getDevice",
          "request": {
            "url": "http://example.com/api/?Action=GetDevice?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a unique device type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02d2b6ed-bfb2-4293-81b5-4247c2bb2626"
            }
          ]
        },
        {
          "id": "6ceee6c8-fab1-4e0d-9070-8d208456c173",
          "name": "listDevices",
          "request": {
            "url": "http://example.com/api/?Action=ListDevices?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about unique device types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "995e1a90-b259-489b-9e05-2717ff867f18"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "7e0d03d7-68b2-4e4f-b1d7-5516835eaba5",
          "name": "getJob",
          "request": {
            "url": "http://example.com/api/?Action=GetJob?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "715e0cc3-338d-4f61-9e32-ef293e97546e"
            }
          ]
        },
        {
          "id": "08364a74-cc15-489b-9a00-03d8e55eb561",
          "name": "listJobs",
          "request": {
            "url": "http://example.com/api/?Action=ListJobs?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about jobs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82b5142e-f1d4-4819-b0a3-3d0b08a0e535"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Status",
      "item": [
        {
          "id": "9b18ddd0-b588-4f4e-af73-9a20c0f0e6b3",
          "name": "getOfferingStatus",
          "request": {
            "url": "http://example.com/api/?Action=GetOfferingStatus?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the current status and future status of all offerings purchased by an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14c621ad-59c0-4102-bb1d-8701a680140d"
            }
          ]
        }
      ]
    },
    {
      "name": "Suites",
      "item": [
        {
          "id": "56adf314-f834-4835-8328-6d023dae93a9",
          "name": "getSuite",
          "request": {
            "url": "http://example.com/api/?Action=GetSuite?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a suite."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9972bf6-aa5e-4b6e-84c5-7c3458a42a1b"
            }
          ]
        },
        {
          "id": "ff1c658e-984e-4a4b-bd5e-3a2c1fa9bf41",
          "name": "listSuites",
          "request": {
            "url": "http://example.com/api/?Action=ListSuites?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about suites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81abcaf6-1b69-4f84-ab37-086727281e10"
            }
          ]
        }
      ]
    },
    {
      "name": "Tests",
      "item": [
        {
          "id": "d7ec9c95-a3f2-44af-bfc0-9e153ca305a1",
          "name": "getTest",
          "request": {
            "url": "http://example.com/api/?Action=GetTest?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a test."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b607c714-ba2f-40c6-9752-f45feeab55c0"
            }
          ]
        },
        {
          "id": "160cd413-6069-436b-8375-232387b4d56a",
          "name": "listTests",
          "request": {
            "url": "http://example.com/api/?Action=ListTests?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about tests."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cf4b2c7-bd7c-45ec-9bc4-68720a1c1c40"
            }
          ]
        }
      ]
    },
    {
      "name": "Artifacts",
      "item": [
        {
          "id": "2a229c8e-053c-434a-83e2-bc2e3879ea87",
          "name": "listArtifacts",
          "request": {
            "url": "http://example.com/api/?Action=ListArtifacts?arn=arn&nextToken=nextToken&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about artifacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48b54c6c-2167-48d6-92e3-f070a63f1720"
            }
          ]
        }
      ]
    },
    {
      "name": "Offerings",
      "item": [
        {
          "id": "9386d650-434e-473b-a0b2-5583b50c9376",
          "name": "listOfferings",
          "request": {
            "url": "http://example.com/api/?Action=ListOfferings?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of products or offerings that the user can manage through the API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45ac6a43-40cf-4be8-bba5-1a4c8d8d5081"
            }
          ]
        },
        {
          "id": "2ca220bf-6fdd-4509-8183-1111ad449c38",
          "name": "purchaseOffering",
          "request": {
            "url": "http://example.com/api/?Action=PurchaseOffering?offeringId=offeringId&quantity=quantity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Immediately purchases offerings for an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6112a4a9-cf5e-45da-af0a-8cac4584cd1a"
            }
          ]
        },
        {
          "id": "8aa14cf7-7c63-42c4-82b1-a5f1062227dc",
          "name": "renewOffering",
          "request": {
            "url": "http://example.com/api/?Action=RenewOffering?offeringId=offeringId&quantity=quantity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Explicitly sets the quantity of devices to renew for an offering, starting from the\n      effectiveDate of the next period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99526b93-9098-4ddc-a07d-917dcc0ddffa"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Transactions",
      "item": [
        {
          "id": "8c4dde00-4ad6-4588-86e0-a7c4bfad69ef",
          "name": "listOfferingTransactions",
          "request": {
            "url": "http://example.com/api/?Action=ListOfferingTransactions?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all historical purchases, renewals, and system renewal transactions for an\n      AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d5d9eb2-2f6d-46f9-8730-7d292c0b8132"
            }
          ]
        }
      ]
    },
    {
      "name": "Samples",
      "item": [
        {
          "id": "7bda1654-032d-4bfa-acde-6f4d27446b11",
          "name": "listSamples",
          "request": {
            "url": "http://example.com/api/?Action=ListSamples?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about samples, given an AWS Device Farm project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17d9a9a8-4f7a-4187-b155-365d6a4bda10"
            }
          ]
        }
      ]
    },
    {
      "name": "Unique Problems",
      "item": [
        {
          "id": "34e4625d-004c-4e7e-a6f1-283028578982",
          "name": "listUniqueProblems",
          "request": {
            "url": "http://example.com/api/?Action=ListUniqueProblems?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about unique problems."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4b65725-e37f-4652-97a2-35972d44fed0"
            }
          ]
        }
      ]
    }
  ]
}