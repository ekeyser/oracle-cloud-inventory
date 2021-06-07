oracle-cloud-inventory
========

#### Oracle Cloud Infrastructure Inventory ####

This module provides an abstraction layer to inventory your cloud resources.

Supported services (and APIs):

Supported Regions
`us-west-1`

### Installation ###
```bash
npm install oracle-cloud-inventory
```

### Usage ###

```javascript
import OracleCloudInventory from 'oracle-cloud-inventory'

const config = {
  credentials: {
    accessKeyId: 'your_access_key',
    secretAccessKey: 'your_secret_key'
  },
  services: ['ec2', 'rds'],
  regions: ['us-west-2, us-east-1']
};

const oInventory = new OracleCloudInventory(config);
const oResources = oInventory.inventory();
```
