{
  "info": {
    "name": "AWS Elastic Load Balancing API Modify Listener",
    "_postman_id": "53a71131-bd42-4480-9db8-f71f9c333a82",
    "description": "Modifies the specified properties of the specified listener.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "bb76993e-f3cf-43ce-ae76-db56020f43eb",
          "name": "addTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?ResourceArns.member.N=ResourceArns.member.N&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the specified tags to the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a4de5fe-d9ee-42e9-acf1-6bccad25b09d"
            }
          ]
        },
        {
          "id": "3697c339-74ba-4d3b-b93d-f7fb3361081a",
          "name": "describeTags",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTags?ResourceArns.member.N=ResourceArns.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the tags for the specified resources."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bd7ccd1-a19f-4e31-a29e-84a676638449"
            }
          ]
        }
      ]
    },
    {
      "name": "Listeners",
      "item": [
        {
          "id": "329b3381-ed11-474e-ad26-c9ff9cc4ca3f",
          "name": "createListener",
          "request": {
            "url": "http://example.com/api/?Action=CreateListener?Certificates.member.N=Certificates.member.N&DefaultActions.member.N=DefaultActions.member.N&LoadBalancerArn=LoadBalancerArn&Port=Port&Protocol=Protocol&SslPolicy=SslPolicy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a listener for the specified Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82d26169-162b-474f-9004-6c4ded2bb43b"
            }
          ]
        },
        {
          "id": "7e0b862b-81d6-4691-8872-dd7450e49934",
          "name": "deleteListener",
          "request": {
            "url": "http://example.com/api/?Action=DeleteListener?ListenerArn=ListenerArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified listener."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "224fa336-d54f-4ccc-8a88-296a5373ae73"
            }
          ]
        },
        {
          "id": "06ba2f50-e922-47d9-beb2-be400fd8b055",
          "name": "describeListeners",
          "request": {
            "url": "http://example.com/api/?Action=DescribeListeners?ListenerArns.member.N=ListenerArns.member.N&LoadBalancerArn=LoadBalancerArn&Marker=Marker&PageSize=PageSize",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified listeners or the listeners for the specified Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c657499b-8854-4ae1-a020-7738b919fc39"
            }
          ]
        },
        {
          "id": "a1d2a607-1178-4229-b48d-b2aa3fc0c7c3",
          "name": "modifyListener",
          "request": {
            "url": "http://example.com/api/?Action=ModifyListener?Certificates.member.N=Certificates.member.N&DefaultActions.member.N=DefaultActions.member.N&ListenerArn=ListenerArn&Port=Port&Protocol=Protocol&SslPolicy=SslPolicy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the specified properties of the specified listener."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a9257eb-b631-45a9-a0cf-c0303a439c30"
            }
          ]
        }
      ]
    },
    {
      "name": "Load Balancers",
      "item": [
        {
          "id": "c5df4619-66b2-442c-887d-0be56bca5692",
          "name": "createLoadBalancer",
          "request": {
            "url": "http://example.com/api/?Action=CreateLoadBalancer?Name=Name&Scheme=Scheme&SecurityGroups.member.N=SecurityGroups.member.N&Subnets.member.N=Subnets.member.N&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94d7b2cc-9e4d-4bd8-9264-2a64448260b8"
            }
          ]
        },
        {
          "id": "c21bf674-0d08-487a-a00d-e1e740b6ce44",
          "name": "deleteLoadBalancer",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLoadBalancer?LoadBalancerArn=LoadBalancerArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Application Load Balancer and its attached listeners."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c2e0db3-1c56-4b83-a6b2-05e3b86dee95"
            }
          ]
        },
        {
          "id": "f16cbe17-9d16-42d4-bf80-b1ed2957e4b8",
          "name": "describeLoadBalancerAttributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBalancerAttributes?LoadBalancerArn=LoadBalancerArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the attributes for the specified Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af2a945c-4228-4b5a-a151-a281096f16c8"
            }
          ]
        },
        {
          "id": "d448818e-5098-4b2a-94c8-99399aef9bea",
          "name": "describeLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBalancers?LoadBalancerArns.member.N=LoadBalancerArns.member.N&Marker=Marker&Names.member.N=Names.member.N&PageSize=PageSize",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified Application Load Balancers or all of your Application Load Balancers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "780cdc78-27cc-4a18-9101-57510d972ef8"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules",
      "item": [
        {
          "id": "b50e18d8-1019-4959-bbad-765fccfb5dc2",
          "name": "createRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateRule?Actions.member.N=Actions.member.N&Conditions.member.N=Conditions.member.N&ListenerArn=ListenerArn&Priority=Priority",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a rule for the specified listener."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad34d3a2-8706-4b3a-80e1-3efc0bda3d19"
            }
          ]
        },
        {
          "id": "61c2ed42-743e-46cf-95ae-88372f14e68c",
          "name": "deleteRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRule?RuleArn=RuleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "262aaaa6-87e3-49f3-8a5f-2baa9980e58e"
            }
          ]
        },
        {
          "id": "3242c3b4-b23a-45ba-85f0-40c45c7c9e16",
          "name": "describeRules",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRules?ListenerArn=ListenerArn&RuleArns.member.N=RuleArns.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified rules or the rules for the specified listener."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2cbe4b96-d440-4ea9-9821-64a5243e070b"
            }
          ]
        }
      ]
    },
    {
      "name": "Target Groups",
      "item": [
        {
          "id": "a84f726b-52f4-43ab-9237-c98dc4520695",
          "name": "createTargetGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateTargetGroup?HealthCheckIntervalSeconds=HealthCheckIntervalSeconds&HealthCheckPath=HealthCheckPath&HealthCheckPort=HealthCheckPort&HealthCheckProtocol=HealthCheckProtocol&HealthCheckTimeoutSeconds=HealthCheckTimeoutSeconds&HealthyThresholdCount=HealthyThresholdCount&Matcher=Matcher&Name=Name&Port=Port&Protocol=Protocol&UnhealthyThresholdCount=UnhealthyThresholdCount&VpcId=VpcId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0cd29dfb-e11e-4e89-8f85-115a1664d221"
            }
          ]
        },
        {
          "id": "4b34874c-4721-4050-a551-043d86a02383",
          "name": "deleteTargetGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTargetGroup?TargetGroupArn=TargetGroupArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5cf7ba4-3192-434f-b19d-9f8f61a1adb5"
            }
          ]
        },
        {
          "id": "11804eb5-a161-4416-bb20-b63fb4afc785",
          "name": "describeTargetGroupAttributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTargetGroupAttributes?TargetGroupArn=TargetGroupArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the attributes for the specified target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32816906-22c3-463d-a1dc-a5b9a01de497"
            }
          ]
        },
        {
          "id": "fbc985ca-a97a-4845-84b8-169f7f1e596e",
          "name": "describeTargetGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTargetGroups?LoadBalancerArn=LoadBalancerArn&Marker=Marker&Names.member.N=Names.member.N&PageSize=PageSize&TargetGroupArns.member.N=TargetGroupArns.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified target groups or all of your target groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed125b44-5ee9-496f-8985-f4329ef1a19e"
            }
          ]
        }
      ]
    },
    {
      "name": "Targets",
      "item": [
        {
          "id": "f60315d7-d394-418a-8031-d01dd2085dc8",
          "name": "deregisterTargets",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTargets?TargetGroupArn=TargetGroupArn&Targets.member.N=Targets.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters the specified targets from the specified target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e046cab8-87f7-4f25-8403-f8128519776a"
            }
          ]
        }
      ]
    },
    {
      "name": "SSL Policies",
      "item": [
        {
          "id": "cbe1a4ea-ed21-4e5c-8346-695acbdc353a",
          "name": "describeSSLPolicies",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSSLPolicies?Marker=Marker&Names.member.N=Names.member.N&PageSize=PageSize",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified policies or all policies used for SSL negotiation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8af2f0dd-944e-41ac-8566-3ce396bd4236"
            }
          ]
        }
      ]
    },
    {
      "name": "Target Health",
      "item": [
        {
          "id": "238c9ddc-1e37-44b5-aff9-64418b0a2ead",
          "name": "describeTargetHealth",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTargetHealth?TargetGroupArn=TargetGroupArn&Targets.member.N=Targets.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the health of the specified targets or all of your targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9a98292-8f04-4a89-a0e6-7cce8b648a30"
            }
          ]
        }
      ]
    }
  ]
}