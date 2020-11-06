**Example 1: Unbinding a direct connect gateway from a NAT Gateway**



Input: 

```
tccli vpc DisassociateDirectConnectGatewayNatGateway --cli-unfold-argument  \
    --VpcId "vpc-8xpno8ee" \
    --DirectConnectGatewayId "dcg-fxa6gh5t" \
    --NatGatewayId "nat-ig8xpno8"
```

Output: 
```
{
    "Response": {
        "RequestId": "dbffc3f0-1807-4683-89ee-2d2b96425ee1"
    }
}
```
