# Exercise 1: Querying the Key Management System

A KMS (Key Management System) stores and manages keys created by a QKD service
One established protocol for communicating with a KMS is the ETSI 014 standard

Two KMS instances are running at:

```text
http://tii-qkd-workshop.uaenorth.cloudapp.azure.com
```

[ETSI 014](https://www.etsi.org/deliver/etsi_gs/QKD/001_099/014/01.01.01_60/gs_qkd014v010101p.pdf)

| Role | SAE ID | Port |
| --- | --- | --- |
| Master | `K002X001` | `5001` |
| Slave | `K002X002` | `5002` |

## Task

Develop a key retrieval client that interacts with the KMS and implements the following API calls

| No. | Method name | URL | Access method |
| --- | --- | --- | --- |
| 1 | Get status | `http://{KME_hostname}/api/v1/keys/{slave_SAE_ID}/status` | `GET` |
| 2 | Get key | `http://{KME_hostname}/api/v1/keys/{slave_SAE_ID}/enc_keys` | `POST` or `GET` |
| 3 | Get key with key IDs | `http://{KME_hostname}/api/v1/keys/{master_SAE_ID}/dec_keys` | `POST` or `GET` |

## Subtasks

To complete the task, be able to answer and complete the following subtasks:

1. How many keys are in the KMS?
2. Retrieve any key in JSON format
3. Retrieve the key with ID `f7e0edef-8bf4-43b2-983b-1e9d22ca6f13`
