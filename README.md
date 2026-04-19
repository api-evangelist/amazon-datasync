# Amazon DataSync

AWS DataSync is an online data transfer service that simplifies, automates, and accelerates moving data between on-premises storage systems, AWS storage services, and other cloud storage. DataSync can transfer data at speeds up to 10 times faster than open-source tools using purpose-built multi-threaded network protocol. It supports NFS, SMB, HDFS, S3, EFS, FSx, and more as transfer endpoints.

## APIs

### Amazon DataSync REST API

RESTful API for AWS DataSync enabling management of data transfer tasks, locations, agents, and task executions for automated data movement between on-premises storage systems and AWS cloud storage.

- **Base URL:** https://datasync.amazonaws.com
- **Documentation:** https://docs.aws.amazon.com/datasync/latest/userguide/API_Reference.html
- **OpenAPI:** [openapi/amazon-datasync-api-openapi.yml](openapi/amazon-datasync-api-openapi.yml)

**Tags:** Data Transfer, Migration, Storage, Automation

## Artifacts

| Type | Count | Location |
|------|-------|----------|
| OpenAPI Specs | 1 | [openapi/](openapi/) |
| JSON Schemas | 10 | [json-schema/](json-schema/) |
| JSON Structures | 10 | [json-structure/](json-structure/) |
| Examples | 10 | [examples/](examples/) |
| JSON-LD Contexts | 1 | [json-ld/](json-ld/) |
| Spectral Rules | 1 | [rules/](rules/) |
| Vocabulary | 1 | [vocabulary/](vocabulary/) |
| Naftiko Capabilities | 2 | [capabilities/](capabilities/) |

## Features

- **High-Speed Data Transfer** — Transfer data at speeds up to 10 times faster than open-source tools using purpose-built multi-threaded network protocol over TLS.
- **Multi-Protocol Support** — Connect to NFS, SMB, HDFS, Amazon S3, Amazon EFS, FSx for Windows, FSx for Lustre, and FSx for NetApp ONTAP as transfer endpoints.
- **Automated Data Validation** — Automatically verify data integrity using checksums at both source and destination to ensure byte-for-byte data consistency after transfer.
- **Scheduled Transfers** — Configure recurring scheduled transfers on hourly, daily, or weekly cadences for ongoing data synchronization between systems.
- **On-Premises Agent** — Deploy the DataSync agent VM on-premises to connect local NFS and SMB storage to AWS without opening inbound firewall ports.
- **Bandwidth Throttling** — Control the network bandwidth consumed by DataSync transfers to minimize impact on production workloads during business hours.
- **CloudWatch Integration** — Monitor transfer metrics, task execution history, and set up alarms for failed transfers using Amazon CloudWatch.

## Use Cases

- **Data Center Migration** — Migrate petabytes of data from on-premises NAS and SAN systems to Amazon S3 or EFS during cloud adoption and data center exit projects.
- **Ongoing Hybrid Synchronization** — Keep on-premises and cloud storage in sync on a scheduled basis for hybrid cloud architectures and distributed workloads.
- **Backup and Archive to Cloud** — Transfer on-premises file data to Amazon S3 Glacier for cost-effective long-term archival and backup storage.
- **Data Distribution** — Transfer datasets between AWS Regions or across AWS accounts for data sharing, disaster recovery, or multi-region analytics.
- **HPC Data Staging** — Stage large datasets from S3 or on-premises storage to FSx for Lustre for high-performance computing workloads on AWS.

## Integrations

- **Amazon S3** — Primary cloud storage destination supporting all S3 storage classes including Glacier for cost-effective data archival.
- **Amazon EFS** — Transfer data to and from Amazon Elastic File System for shared file storage accessible from multiple EC2 instances.
- **Amazon FSx** — Integrate with FSx for Windows, FSx for Lustre, and FSx for NetApp ONTAP as high-performance managed file system destinations.
- **Amazon CloudWatch** — Receive DataSync task execution metrics, transfer rates, and error alerts in CloudWatch for monitoring and incident response.
- **AWS Snowball** — Use Snowball for initial bulk data transfer followed by DataSync for ongoing incremental synchronization after migration.
- **AWS Storage Gateway** — Combine Storage Gateway for cache-based hybrid access with DataSync for bulk data movement between on-premises and cloud.

## Resources

- [Portal](https://aws.amazon.com/datasync/)
- [Documentation](https://docs.aws.amazon.com/datasync/)
- [Getting Started](https://aws.amazon.com/datasync/getting-started/)
- [Pricing](https://aws.amazon.com/datasync/pricing/)
- [FAQ](https://aws.amazon.com/datasync/faqs/)
- [Blog](https://aws.amazon.com/blogs/storage/)
- [GitHub Organization](https://github.com/aws)
- [Console](https://console.aws.amazon.com/datasync/)
- [Support](https://aws.amazon.com/premiumsupport/)
- [Terms of Service](https://aws.amazon.com/service-terms/)
- [Privacy Policy](https://aws.amazon.com/privacy/)

## Maintainers

- **Kin Lane** — kin@apievangelist.com
