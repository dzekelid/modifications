---
swagger: "2.0"
x-collection-name: AWS Elastic Load Balancing
x-complete: 1
info:
  title: AWS Elastic Load Balancing API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ModifyListener:
    get:
      summary: Modify Listener
      description: Modifies the specified properties of the specified listener.
      operationId: modifyListener
      x-api-path-slug: actionmodifylistener-get
      parameters:
      - in: query
        name: Certificates.member.N
        description: The SSL server certificate
        type: string
      - in: query
        name: DefaultActions.member.N
        description: The default actions
        type: string
      - in: query
        name: ListenerArn
        description: The Amazon Resource Name (ARN) of the listener
        type: string
      - in: query
        name: Port
        description: The port for connections from clients to the load balancer
        type: string
      - in: query
        name: Protocol
        description: The protocol for connections from clients to the load balancer
        type: string
      - in: query
        name: SslPolicy
        description: The security policy that defines which ciphers and protocols
          are supported
        type: string
      responses:
        200:
          description: OK
      tags:
      - Listeners
  /?Action=ModifyLoadBalancerAttributes:
    get:
      summary: Modify Load Balancer Attributes
      description: Modifies the specified attributes of the specified Application
        Load Balancer.
      operationId: modifyLoadBalancerAttributes
      x-api-path-slug: actionmodifyloadbalancerattributes-get
      parameters:
      - in: query
        name: Attributes.member.N
        description: The load balancer attributes
        type: string
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=ModifyRule:
    get:
      summary: Modify Rule
      description: Modifies the specified rule.
      operationId: modifyRule
      x-api-path-slug: actionmodifyrule-get
      parameters:
      - in: query
        name: Actions.member.N
        description: The actions
        type: string
      - in: query
        name: Conditions.member.N
        description: The conditions
        type: string
      - in: query
        name: RuleArn
        description: The Amazon Resource Name (ARN) of the rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rules
  /?Action=ModifyTargetGroup:
    get:
      summary: Modify Target Group
      description: Modifies the health checks used when evaluating the health state
        of the targets in the specified target group.
      operationId: modifyTargetGroup
      x-api-path-slug: actionmodifytargetgroup-get
      parameters:
      - in: query
        name: HealthCheckIntervalSeconds
        description: The approximate amount of time, in seconds, between health checks
          of an individual target
        type: string
      - in: query
        name: HealthCheckPath
        description: The ping path that is the destination for the health check request
        type: string
      - in: query
        name: HealthCheckPort
        description: The port to use to connect with the target
        type: string
      - in: query
        name: HealthCheckProtocol
        description: The protocol to use to connect with the target
        type: string
      - in: query
        name: HealthCheckTimeoutSeconds
        description: The amount of time, in seconds, during which no response means
          a failed health check
        type: string
      - in: query
        name: HealthyThresholdCount
        description: The number of consecutive health checks successes required before
          considering an unhealthy target healthy
        type: string
      - in: query
        name: Matcher
        description: The HTTP codes to use when checking for a successful response
          from a target
        type: string
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      - in: query
        name: UnhealthyThresholdCount
        description: The number of consecutive health check failures required before
          considering the target unhealthy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Target Groups
  /?Action=ModifyTargetGroupAttributes:
    get:
      summary: Modify Target Group Attributes
      description: Modifies the specified attributes of the specified target group.
      operationId: modifyTargetGroupAttributes
      x-api-path-slug: actionmodifytargetgroupattributes-get
      parameters:
      - in: query
        name: Attributes.member.N
        description: The attributes
        type: string
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Target Groups
---