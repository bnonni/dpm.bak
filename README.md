# DPM

```ts
import * as Web5 from 'did:dht:123/package/api/0.1.0'
```

* Idea: how to lookup did using a naming convention
* E.g. '@web5/api' => 'did:dht:web5/package/api'

* dpm.lock
  * produced after install
  * contains modified version of the install path
  * locks the version to the hash of the data
  * contains the path of the DMI@hash-of-the-content-at-that-recordId
* <https://hackmd.io/dtS5CgUuQIK3_n6hbK4jFA>

```ts
{
    "did:dht:123/package/api/0.1.0": {
        "version": "0.1.0",
        "resolved": "http://dweb/did:dht:123/protocols/dpm/package/api/0.1.0",
        "integrity": "sha512-HazVq9zwTVwGmqdwYzu7WyQ6FQVZ7SwET0KKQuKm55jD0IfUpZgN0OPIiZG3zV1iSrVYcN0bdwLRXI/VNCYsUA==",
        "license": "Apache-2.0"
    }
}
```

* DIDs are entities: org or user
* DMI: Decentralized Module Import
* <https://github.com/TBD54566975/web5-js/blob/main/packages/api/src/web-features.ts>
* TAB Conf
  * Install DPM setting up env script
  * dpm install
  * push update
  * dpm install again
