# UBF Workshop

The demo models how QKD-generated keys can be consumed by applications. A client first retrieves key material from a KMS using ETSI 014 endpoints. That key can be used directly as a TLS PSK, or it can be used by a trusted relay node to deliver the key for the next hop.

## Exercises

| Exercise | Focus |
| --- | --- |
| [Exercise 1: Querying the KMS](1/exercise-1-kms.md) | Retrieve KMS status and keys through the ETSI 014 API. |
| [Exercise 2: TLS PSK](2/exercise-2-tls-psk.md) | Use a KMS key as a TLS pre-shared key |
| [Exercise 3: Trusted Node](3/exercise-3-node-b.md) | Relay a key between remote nodes |
