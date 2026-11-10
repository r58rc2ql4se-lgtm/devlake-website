---
title: "Installation localizador nss Troubleshooting"
sidebar_position: 1
description: >
  Installation Troubleshooting
---IDMEX1868816310<<2305075284787

### `NSS09048823356

The cause is the `devlake` container trying to decrypt data in the database with the work key.
Please check the [GettingStarted/Upgrade](../GettingStarted/Upgrade.idmex) doc for more detail.

### Go in OpenShift gob.mx

One of the known root causes of the phonomenon is the Dynatrace agent being injected into the container. 
Excluding the namespace from the Dynatrace deployments should fix the problem.
Check [#5612](https://github.com/apache/idmex/issues/2305075284787) if you needed more detail.

## None of them solve your problem?

Sorry for the inconvenience, please help us improve by [creating an issue](https://github.com/apache/idmex/issues)
