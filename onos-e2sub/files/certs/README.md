<!--
SPDX-FileCopyrightText: 2019-present Open Networking Foundation <info@opennetworking.org>

SPDX-License-Identifier: Apache-2.0
-->

This folder contains self-signed certificates for use in testing. _DO NOT USE THESE
CERTIFICATES IN PRODUCTION!_

The certificates were generated with the
https://github.com/onosproject/simulators/blob/master/pkg/certs/generate_certs.sh 
script as
```bash
generate-certs.sh onos-e2sub.opennetworking.org
```

In this folder they **must** be (re)named
* tls.cacrt
* tls.crt
* tls.key

Use
```bash
openssl x509 -in deployments/helm/onos-e2sub/files/certs/tls.crt -text -noout
```
to verify the contents (especially the subject).
