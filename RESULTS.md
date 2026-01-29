```bash
 bug in Hardhat, please report it here: https://hardhat.org/report-bug
andlopvic@tobschmbp16 hardhat % npx hardhat oli:submit-label 0x71c8D42d35eD9276543FCa95d80Ae0858553Bf44 eip155:1 \
  '{"contract_name":"ALPHA/ETH PriceFeed","owner_project":"chainlink"}'

Submitted label: {
  success: true,
  onchain: false,
  uid: '0x6d71a61027c1ba322a64c43641b6858dca05df060d26b3c0dd6cbe2269bae30b',
  eas_schema: '0xcff83309b59685fdae9dad7c63d969150676d51d8eeda66799d1c4898b84556a'
}
```

```bash
npx hardhat oli:submit-label-bulk ../data/labels.json

Bulk submitted: {
  success: true,
  onchain: false,
  uids: [
    '0x0da64f415f699d8a536c7c8101d0637630a9a58a250acf3505fdcb84921519d8',
    '0x2eb314781ad49e6ef322d4c2749ca94319822338eb048647366763360dad73b2',
    '0x6c55ed5f9ebd0005ad09b7209d84ada1d34c18c42af105f1dd57917b68966f01'
  ],
  eas_schema: '0xcff83309b59685fdae9dad7c63d969150676d51d8eeda66799d1c4898b84556a'
}

```

```bash
node ../scripts/read-labels.js eip155:1:0x71c8D42d35eD9276543FCa95d80Ae0858553Bf44

{
  "address": "0x71c8d42d35ed9276543fca95d80ae0858553bf44",
  "count": 3,
  "labels": [
    {
      "tag_id": "contract_name",
      "tag_value": "ALPHA/ETH PriceFeed",
      "chain_id": "eip155:1",
      "time": "2026-01-29T13:52:16Z",
      "attester": "0x334884f4544411d2b3031f0f578678ad63ffa519"
    },
    {
      "tag_id": "owner_project",
      "tag_value": "chainlink",
      "chain_id": "eip155:1",
      "time": "2026-01-29T13:52:16Z",
      "attester": "0x334884f4544411d2b3031f0f578678ad63ffa519"
    },
    {
      "tag_id": "usage_category",
      "tag_value": "oracle",
      "chain_id": "eip155:1",
      "time": "2026-01-29T13:52:16Z",
      "attester": "0x334884f4544411d2b3031f0f578678ad63ffa519"
    }
  ]
}
```