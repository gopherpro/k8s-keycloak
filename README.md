<img src="https://camo.githubusercontent.com/5b298bf6b0596795602bd771c5bddbb963e83e0f/68747470733a2f2f692e696d6775722e636f6d2f7031527a586a512e706e67" align="left" width="110px" height="110px"/>

# k8s-keycloak

_... managed by Flux and serviced with RenovateBot_ :robot:

## :book: Overview

K3s cluster running Keycloak and managed by Flux2.

## :lock_with_ink_pen: Secret management

Secrets are encrypted using [sops](https://github.com/mozilla/sops) before being pushed into this repository.
The encrypted secrets are then decrypted by sops using the private key inside the cluster.

## :gear: Automation

- [Renovatebot](https://github.com/renovatebot/renovate) keeps my applications up-to-date by scanning my repo and opening pull requests when it notices a new container image update.