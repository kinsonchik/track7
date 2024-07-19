Hardware requirements
=====================

Last Updated: 2024-06-27

Before you install IBM Cloud Pak for Data, review the hardware requirements for the control plane, the shared cluster components, and the services that you plan to install.

|Components|Related links|
| --- | --- |
| [Cloud Pak for Data platform hardware requirements](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform) | Review the minimum requirements for a stable installation: 
-   [Cloud Pak for Data platform hardware requirements](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform)

Work with your IBM Sales representative to determine whether you need more resources based on:

-   The shared cluster components that you need to install.
-   The services that you plan to install.
-   The types of workloads that you plan to run.

In addition, review the following resources:

-   [Cluster node settings](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__settings)
-   [Disk requirements](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__disk)

|
| [Shared cluster-wide components](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__shared) | Review the hardware requirements for the shared cluster components that you need to install.

-   [x86-64 hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__shared-x86)
-   [IBM Power (ppc64le) hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__shared-power)
-   [Z (s390x) hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__shared-z)

 |
| [Instance-level prerequisites](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__instance-prereq) | Review the hardware requirements for the instance-level prerequisites.

-   [x86-64 hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__instance-prereq-x86)
-   [IBM Power (ppc64le) hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__instance-prereq-power)
-   [Z (s390x) hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__instance-prereq-z)

 |
| [Services](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__services) | Review the hardware requirements for the services that you plan to install.

-   [x86-64 hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__svc-x86)
-   [IBM Power (ppc64le) hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__svc-power)
-   [Z (s390x) hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__svc-z)

Not all services are supported on all hardware.

 |
| [Automatically installed dependencies](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__auto) | Review the hardware requirements for the automatically installed dependencies, such as the common core services. (These components are installed only if you install a service with a dependency on the component.)

-   [x86_64 hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__x86-auto)
-   [Power (ppc64le) hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__ppc-auto)
-   [Z (s390x) hardware](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__z-auto)

 |

Cloud Pak for Data platform hardware requirements[](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform__title__1 "Copy to clipboard")
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

You must install Cloud Pak for Data on a Red Hat® OpenShift® Container Platform cluster. For information about the supported versions of Red Hat OpenShift Container Platform, see [Software requirements](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/software-reqs.html "Before you install IBM Cloud Pak for Data, review the software requirements for the control plane, the shared cluster components, and the services that you plan to install, and review the supported web browsers.").

It is strongly recommended that you deploy Cloud Pak for Data on a highly available cluster. If you plan to install Cloud Pak for Data on a highly available cluster, review [Highly available deployments](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__ee-se-reqs).

If high availability is not a requirement for your deployment, you can deploy Cloud Pak for Data on a single node OpenShift (SNO) cluster. If you plan to install Cloud Pak for Data on SNO, review [Single node OpenShift deployments](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__sno).

* * * * *

Highly available deployments

-   [](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/required-components.html)
-   [](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-nav/head/services.html)

    [](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/hardware-reqs.html#hardware-reqs__services)

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/downloading-scaling-pdf.html "Detailed component sizing guidance is available in a PDF file that you can download from the IBM Entitled Registry.")

|  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/storage-requirements.html#compute-requirements__platform-storage)

 |
|  |  |  |  |  |  |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/hardware-reqs.html#hardware-reqs__services__title__1)

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/hardware-reqs.html#hardware-reqs__services__title__1)

* * * * *

* * * * *

Single node OpenShift deployments

-   [](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/remote-physical-locations.html)

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/admin/backup_restore.html)

-   [](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-nav/head/services.html)

    [](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/hardware-reqs.html#hardware-reqs__services)

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/downloading-scaling-pdf.html "Detailed component sizing guidance is available in a PDF file that you can download from the IBM Entitled Registry.")

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
|  |  |  |  |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/storage-requirements.html#compute-requirements__platform-storage)

 |

* * * * *

Cluster node settings[](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__settings__title__1 "Copy to clipboard")
---------------------------------------------------------------------------------------------------------------------------------------------------------------

The time on all of the nodes must be synchronized within 500 ms.

Some services require additional node settings to run correctly. For information about the node settings and the services that require them, see [Changing required node settings](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/install/prep-cluster-node-settings.html). You must change the node settings before you install Cloud Pak for Data.

Disk requirements[](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__disk__title__1 "Copy to clipboard")
-------------------------------------------------------------------------------------------------------------------------------------------------------

To prepare your storage disks, ensure that you have good I/O performance, and prepare the disks for encryption.

I/O performance

When I/O performance is not sufficient, services can experience poor performance or cluster instability, such as functional failures with timeouts. This is especially true when you are running a heavy workload.

To assess your I/O performance:

1.  Run the Cloud Pak for Data [storage performance validation playbook](https://www.ibm.com/links?url=https%3A%2F%2Fgithub.com%2FIBM%2Fk8s-storage-perf "(Opens in a new tab or window)") on the cluster where you plan to install Cloud Pak for Data and compare your results with the recommendations.

    The I/O performance requirements for Cloud Pak for Data are based on extensive testing in various cloud environments. The tests validate the I/O performance in these environments. The requirements are based on the performance of writing data to representative storage classes using the following block size and thread count combinations.

    -   To evaluate disk latency, the I/O tests use a small block (4 KB) with 8 threads.
    -   To evaluate disk throughput, the I/O tests use a large block (1 GB) with 2 threads.

    Ensure that the results of the storage performance validation playbook are comparable to the following recommended minimum values.

    Disk latency (4 KB block with 8 threads)

    For disk latency tests, 11 MB/s has been found to provide sufficient performance.

    Disk throughput (1 GB block with 2 thread)

    For disk throughput tests, 128 MB/s has been found to provide sufficient performance.

    To ensure sufficient performance, both requirements should be satisfied; however, this might not be feasible in all environments.

    Some storage types might have more stringent I/O requirements. For details, see [Storage considerations](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/storage_considerations.html).

    Important: It is recommended that you run the validation playbook several times to account for variations in workloads, access patterns, and network traffic.

    In addition, if your storage volumes are remote, network speed can be a key factor in your I/O performance. For good I/O performance, ensure that you have sufficient network speed, as described in [Storage considerations](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/storage_considerations.html).

2.  Complete a proof of concept with representative workloads.

    If your proof of concept encounters functional issues or performance issues, determine the root cause of the problem to confirm whether the issue is related to I/O performance. You can use the following best practices to help identify potential problems.

    -   [Performing routine IBM Cloud Pak for Data monitoring](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/admin/best-practice-routine-cpd-monitoring.html)
    -   [Performing routine cluster monitoring](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/admin/best-practice-routine-cluster-monitoring.html)

Workloads can vary dramatically in terms of complexity and concurrency. As you assess your I/O performance, apply the following information:

-   If you are unable to satisfy the recommended I/O performance requirements, you run a high risk of encountering performance problems.
-   As the gap between your measured I/O performance and the recommended I/O performance widens, you run an increased risk of performance and functional issues. For example, if disk latency-based measurement is around or under 2 MB/s, you are likely to have all kinds of performance and functional issues. In this case, I/O performance should be improved before you proceed.

    However, if disk latency-based measurement is approximately 5 MB/s or higher, you can proceed. In this case, continue to monitor workloads closely and consider improving I/O performance.

-   As your workloads increase, you can work with your infrastructure or storage vendor to review and improve I/O performance to ensure that it remains sufficient and optimal.

Encryption with Linux® Unified Key Setup (LUKS2)

To ensure that your data within Cloud Pak for Data is stored securely, you can encrypt your disks when you install Red Hat OpenShift Container Platform. For more information, see *Encrypting and mirroring disks during installation* in the Red Hat OpenShift Container Platform documentation:

-   [Version 4.12](https://docs.openshift.com/container-platform/4.12/installing/install_config/installing-customizing.html#installation-special-config-storage_installing-customizing "(Opens in a new tab or window)")
-   [Version 4.14](https://docs.openshift.com/container-platform/4.14/installing/install_config/installing-customizing.html#installation-special-config-storage_installing-customizing "(Opens in a new tab or window)")
-   [Version 4.15](https://docs.openshift.com/container-platform/4.15/installing/install_config/installing-customizing.html#installation-special-config-storage_installing-customizing "(Opens in a new tab or window)")

Shared cluster-wide components[](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__shared__title__1 "Copy to clipboard")
----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Shared cluster components provide underlying functionality for the IBM Cloud Pak for Data control plane and services. Use the following sections to understand the hardware requirements for the following components.

-   IBM Certificate manager
-   License Service
-   Scheduling service

For more information, see [Cluster-wide components](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/required-components.html#required-components__cluster-comps).

Use the following information to determine whether you have the minimum required resources to install each component on your cluster.

* * * * *

x86-64 hardware

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  |  |  |  |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/required-components.html#required-components__cluster-comps)

-   [](https://www.ibm.com/docs/SSRV9V_4.7/installer/hardware_sizing_reqs.html "(Opens in a new tab or window)")

 |
|  |  |  |  |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/required-components.html#required-components__cluster-comps)

-   [](https://www.ibm.com/docs/SSRV9V_4.7/installer/hardware_sizing_reqs.html "(Opens in a new tab or window)")

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/required-components.html#required-components__cluster-comps)

 |

* * * * *

* * * * *

IBM Power (ppc64le) hardware

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  |  |  |  |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/required-components.html#required-components__cluster-comps)

-   [](https://www.ibm.com/docs/SSRV9V_4.7/installer/hardware_sizing_reqs.html "(Opens in a new tab or window)")

 |
|  |  |  |  |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/required-components.html#required-components__cluster-comps)

-   [](https://www.ibm.com/docs/SSRV9V_4.7/installer/hardware_sizing_reqs.html "(Opens in a new tab or window)")

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/required-components.html#required-components__cluster-comps)

 |

* * * * *

* * * * *

Z (s390x) hardware

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  |  |  |  |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/required-components.html#required-components__cluster-comps)

-   [](https://www.ibm.com/docs/SSRV9V_4.7/installer/hardware_sizing_reqs.html "(Opens in a new tab or window)")

 |
|  |  |  |  |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/required-components.html#required-components__cluster-comps)

-   [](https://www.ibm.com/docs/SSRV9V_4.7/installer/hardware_sizing_reqs.html "(Opens in a new tab or window)")

 |

* * * * *

Instance-level prerequisites[](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__instance-prereq__title__1 "Copy to clipboard")
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Instance-level prerequisites provide underlying functionality for services. Use the following sections to understand the hardware requirements for:

-   IBM Cloud Pak for Data control plane
-   IBM Cloud Pak foundational services

For more information, see [Instance-level components](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/cpd/plan/required-components.html#required-components__instance-comps).

Use the following information to determine whether you have the minimum required resources to install each component on your cluster.

* * * * *

x86-64 hardware

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  | [](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform) | [](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform) | [](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform) |  |
|  |  |  |

-   [](https://www.ibm.com/docs/SSRV9V_4.7/installer/hardware_sizing_reqs.html "(Opens in a new tab or window)")

 |  |

* * * * *

* * * * *

IBM Power (ppc64le) hardware

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  | [](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform) | [](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform) | [](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform) |  |
|  |  |  |

-   [](https://www.ibm.com/docs/SSRV9V_4.7/installer/hardware_sizing_reqs.html "(Opens in a new tab or window)")

 |  |

* * * * *

* * * * *

Z (s390x) hardware

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  | [](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform) | [](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform) | [](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__platform) |  |
|  |  |  |

-   [](https://www.ibm.com/docs/SSRV9V_4.7/installer/hardware_sizing_reqs.html "(Opens in a new tab or window)")

 |  |

* * * * *

Services[](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__services__title__1 "Copy to clipboard")
--------------------------------------------------------------------------------------------------------------------------------------------------

Use the following information to determine whether you have the minimum required resources to install each service that you want to use.

* * * * *

x86-64 hardware

|

Software

 |

vCPU

 |

Memory

 |

Storage

 |

Notes

 |
| --- | --- | --- | --- | --- |
| AI Factsheets |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
0.3 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
1.2 GB RAM

 |

**Persistent storage:**\
Uses the persistent storage provisioned by the common core services.

**Ephemeral storage:**\
300 GB

**Image storage:**\
Up to 2.42 GB

 |

Minimum resources for an installation with a single replica per service.

 |
| Anaconda Repository for IBM Cloud Pak for Data |

4 vCPU

 | 8 GB RAM | 1 TB | This service cannot be installed on your Red Hat OpenShift cluster. For details, see the [Anaconda installation requirements](https://www.ibm.com/links?url=https%3A%2F%2Fteam-docs.anaconda.com%2Fen%2Flatest%2Fprep%2Fstandard-prep.html%23install-requirements "(Opens in a new tab or window)"). |
| Analytics Engine powered by Apache Spark |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
2.3 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
9 GB RAM

 |

**Persistent storage:**This information is not currently available.

**Ephemeral storage:**\
50 GB per vCPU request\
(SSDs are recommended)

**Image storage:**\
Up to 31.90 GB

 | Spark jobs use `emptyDir` volumes for temporary storage and shuffling. If your Spark jobs use a lot of disk space for temporary storage or shuffling, make sure that you have sufficient space on the local disk where `emptyDir` volumes are created.

The recommended location is a partition in /var/lib. For more information, see *Understanding ephemeral storage*in the Red Hat OpenShift documentation:

-   [Version 4.12](https://docs.openshift.com/container-platform/4.12/storage/understanding-ephemeral-storage.html "(Opens in a new tab or window)")
-   [Version 4.14](https://docs.openshift.com/container-platform/4.14/storage/understanding-ephemeral-storage.html "(Opens in a new tab or window)")
-   [Version 4.15](https://docs.openshift.com/container-platform/4.15/storage/understanding-ephemeral-storage.html "(Opens in a new tab or window)")

If you don't have sufficient space on the local disk, Spark jobs might run slowly and some of the executors might evict jobs. A minimum of 50 GB of temporary storage for each vCPU request is recommended.

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

All of the Analytics Engine powered by Apache Spark service instances associated with an instance of Cloud Pak for Data use the same pool of resources.

 |
| Cognos Analytics |

**Operator pods:**\
0.5 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
9.4 vCPU

 |

**Operator pods:**\
1 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
38.5 GB RAM

 |

**Persistent storage:**

-   500 MB for the service
-   2 GB per instance (smallest instance)

**Ephemeral storage:**

-   1 GB for the service
-   21.6 GB per instance (smallest instance)\
**Image storage:**\
Up to 26.20 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

When you provision the Cognos Analytics service, you specify the size of the instance.

The information here is for the smallest instance. For other sizes, see [Provisioning the Cognos Analytics service](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-cognos/ca-instance.html).

 |
| Cognos Dashboards |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.5 vCPU

**Operand:**\
11 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.256 GB RAM

**Operand:**\
36 GB RAM

 |

**Persistent storage:**\
30 GB

**Ephemeral storage:**\
37.4 GB

**Image storage:**\
Up to 13.77 GB

 |

Minimum resources for an installation with a single replica per service.

 |
| Data Gate |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
2 vCPU per instance

 |

**Operator pods:**\
0.1 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
13 GB RAM per instance

 |

**Persistent storage:**\
50 GB per instance

**Ephemeral storage:**\
0.6 - 3.25 GB

**Image storage:**\
Up to 17.45 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| Data Privacy |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
1 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
3.77 GB RAM

 |

**Persistent storage:**\
Uses the persistent storage provisioned by IBM Knowledge Catalog.

**Ephemeral storage:**\
4.5 GB

**Image storage:**\
Up to 3.15 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| Data Product Hub |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
0.13 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
0.45 GB RAM

 |

**Persistent storage:**\
Uses the persistent storage provisioned by the common core services.

**Ephemeral storage:**\
4.5 GB

**Image storage:**\
Up to 2.47 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| Data Refinery |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.5 vCPU

**Operand:**\
1 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
1 GB RAM

**Operand:**\
4 GB RAM

 |

**Persistent storage:**\
Uses the persistent storage provisioned by the common core services.

**Ephemeral storage:**\
2 GB

**Image storage:**\
Up to 3.78 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

This service is installed when you install IBM Knowledge Catalog or Watson Studio

 |
| Data Replication |

**Operator pods:**\
0.5 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
13 vCPU

 |

**Operator pods:**\
0.512 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
14 GB RAM

 |

**Persistent storage:**\
10 GB - 512 GB

**Ephemeral storage:**\
22 GB

**Image storage:**\
Up to 3.91 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| DataStage |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
8 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
31 GB RAM

 |

**Persistent storage:**\
300 GB

**Ephemeral storage:**This information is not currently available.

**Image storage:**\
Up to 19.72 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

Local storage in /var/lib/containers

Adjust the amount of local storage per node based on the volume of data you are analyzing. Local storage should be approximately 2 times larger than the amount of data you expect the system to process concurrently.

 |
| Data Virtualization |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
12 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
38 GB RAM

 |

**Persistent storage:**\
280 GB total (assuming defaults)

-   **Head pod:**

    50 GB (default)

-   **One worker pod:**

    50 GB (default)

-   **Caching storage:**

    100 GB (default)

-   **Caching metadata:**

    10 GB

-   **Scheduling pod:**

    10 GB

-   **Log storage:**

    30 GB per pod\
**Ephemeral storage:**\
2.428 - 13GB

**Image storage:**\
Up to 2.23 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

When you provision the service, you can specify:

-   The size of the persistent volume for the head pod
-   The size of the persistent volume for the cache
-   The number of worker pods
-   The size of the persistent volume for the worker pods

 |
| Db2 |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
8 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
24 GB RAM

 |

**Persistent storage:**\
540 GB (assuming defaults)

**Ephemeral storage:**\
2.2 - 9.7 GB

**Image storage:**\
Up to 0.64 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

A dedicated node is recommended for production deployments of Db2. For details, see [Setting up dedicated nodes](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-db2/aese-dednodes.html).

 |
| Db2 Big SQL |

**Operator pods:**\
0.2 vCPU

**Catalog pods:**\
0.1 vCPU

**Operand:**\
10.2 vCPU

 |

**Operator pods:**\
0.3 GB RAM

**Catalog pods:**\
0.2 GB RAM

**Operand:**\
66.7 GB RAM

 |

**Persistent storage:**\
470 GB total (assuming defaults)

-   **Head pod:**

    200 GB (default)

-   **One worker pod:**

    200 GB (default)

-   **Scheduling pod:**

    10 GB

-   **Log storage:**

    30 GB per pod\
**Ephemeral storage:**\
1.4 - 12.2 GB

**Image storage:**\
Up to 0.40 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

When you provision the service, you can specify:

-   The resources (vCPU and RAM) for the head and worker pods
-   The number of worker pods
-   The size of the persistent volume for the head pod and worker pods

 |
| Db2 Data Management Console |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
5 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
19.31 GB RAM

 |

**Persistent storage:**\
10 GB

**Ephemeral storage:**\
7.5 GB

**Image storage:**\
Up to 5.89 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

For information on sizing the provisioned instance, see [Creating a service instance for Db2 Data Management Console from the web client](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-dmc/dmc-svc-inst-web.html).

 |
| Db2 Warehouse |

**Operator pods:**\
0.5 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
**SMP:** 7 vCPU\
**MPP:** 39 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
**SMP:** 98 GB RAM\
**MPP:** 610 GB RAM

 |

**Persistent storage:**\
540 GB (assuming defaults)

**Ephemeral storage:**\
2.2 - 10.8 GB

**Image storage:**\
Up to 2.15 GB

 |

Minimum resources for an installation with a single replica per service.

Use dedicated nodes for:

-   Production SMP deployments (recommended)
-   MPP deployments (required)

For detail, see [Setting up dedicated nodes](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-db2w/db2w-dednodes.html).

Development deployment

-   1 node for SMP
-   2 nodes for MPP

Production deployment

-   1 node for SMP
-   2-999 nodes for MPP

Recommended configuration

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| Decision Optimization |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
0.9 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
1.5 GB RAM

 |

**Persistent storage:**\
12 GB

**Ephemeral storage:**\
300 - 6500 MB

**Image storage:**\
Up to 3.29 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| EDB Postgres |

**Operator pods:**\
**IBM:** 0.1 vCPU\
**Third-party:** 0.5 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
User-defined

 |

**Operator pods:**\
**IBM:** 0.256 GB RAM\
**Third-party:** 0.2 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
User-defined

 |

**Persistent storage:**\
100 GB

**Ephemeral storage:**This information is not currently available.

**Image storage:**\
Up to 2.71 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| Execution Engine for Apache Hadoop |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
For each deployment:\
0.5 vCPU +  (0.5 vCPU * number of Hadoop registrations) + (0.6 vCPU * number of Hadoop jobs run)

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
For each deployment:\
0.5 GB + (0.5 GB * number of Hadoop registrations) + (0.5 GB * number of Hadoop jobs run)

 |

**Persistent storage:**\
2 GB per image pushed

**Ephemeral storage:**\
218 - 436 MB

**Image storage:**\
Up to 2.46 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

Each image that is pushed to the remote Hadoop cluster requires disk space where image tgz file can be stored.

Execution Engine for Apache Hadoop requires an Execution Engine for Hadoop RPM installation on the Apache Hadoop cluster. For details, see [Installing the service on Apache Hadoop clusters](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/wsj/install/installing-hadoop-cluster.html).

 |
| IBM Knowledge Catalog |

Base

**Operator pods:**\
0.75 vCPU

**Catalog pods:**\
0.05 vCPU

**Operand:**\
26 vCPU

Data quality

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
11 vCPU

Semantic search and lineage

**Operator pods:**\
1.5 vCPU

**Catalog pods:**\
0.05 vCPU

**Operand:**\
5 vCPU

 |

Base

**Operator pods:**\
4 GB RAM

**Catalog pods:**\
0.2 GB RAM

**Operand:**\
73 GB RAM

Data Quality

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
44 GB RAM

Semantic search and lineage

**Operator pods:**\
0.7 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
20 GB RAM

 |

**Persistent storage:**\
900 GB

**Ephemeral storage:**

Base

840 MB - 19.4 GB

Data quality

105 MB - 2.15 GB

Semantic search and lineage

210 MB - 2.53 GB

**Image storage:**\
Up to 46.95 GB with all optional components

 |

The minimum required resources depend on the features that you install.

If Data Refinery is not installed, add the vCPU and memory required for Data Refinery to the information listed for IBM Knowledge Catalog.

Local storage in /var/lib/containers

Adjust the amount of local storage per node based on the volume of data you are analyzing. Local storage should be approximately 2 times larger than the amount of data you expect the system to process concurrently.

Persistent storage

The raw size of shared storage depends on the storage class you use. For example, if you use `portworx-shared-gp3`, which has 3 replicas, multiply the storage by the number of replicas.

 |
| IBM Knowledge Catalog Premium |

**Operator pods:**\
0.75 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
30 vCPU

 |

**Operator pods:**\
1.5 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
78 GB RAM

 |

**Persistent storage:**\
150 GB

**Ephemeral storage:**\
10 GB

**Image storage:**\
Up to 28.66 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

The service requires one GPU.

GPU support is limited to

-   NVIDIA A100 GPUs with 80 GB RAM
-   NVIDIA H100 GPUs with 80 GB RAM
-   NVIDIA L40S GPUs with 48 GB RAM

Restriction: Do not configure NVIDIA Multi-Instance GPU if you plan to install this service.

 |
| IBM Knowledge Catalog Standard |

**Operator pods:**\
0.75 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
25 vCPU

 |

**Operator pods:**\
1.5 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
61 GB RAM

 |

**Persistent storage:**\
150 GB

**Ephemeral storage:**\
10 GB

**Image storage:**\
Up to 28.66 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

The service requires one GPU.

GPU support is limited to

-   NVIDIA A100 GPUs with 80 GB RAM
-   NVIDIA H100 GPUs with 80 GB RAM
-   NVIDIA L40S GPUs with 48 GB RAM

Restriction: Do not configure NVIDIA Multi-Instance GPU if you plan to install this service.

 |
| IBM Match 360 with Watson |

**Operator pods:**\
2 vCPU

**Catalog pods:**\
1 vCPU

**Operand:**\
28 vCPU

 |

**Operator pods:**\
2 GB RAM

**Catalog pods:**\
2 GB RAM

**Operand:**\
97 GB RAM

 |

**Persistent storage:**\
190 GB

**Ephemeral storage:**\
16 GB

**Image storage:**\
Up to 16.97 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| Informix |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.1 vCPU

**Operand:**\
2 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
2 GB RAM

 |

**Persistent storage:**\
20 GB

**Ephemeral storage:**\
900 MB (default)

**Image storage:**\
Up to 5.47 GB

 |

Minimum resources for an installation with a single replica per service.

 |
| MANTA Automated Data Lineage |

**Operator pods:**\
0.5 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
11 vCPU

 |

**Operator pods:**\
0.5 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
26 GB RAM

 |

**Persistent storage:**\
37 GB

**Ephemeral storage:**\
5 GB

**Image storage:**\
Up to 5.26 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| MongoDB |

**Operator pods:**\
**IBM:** 0.1 vCPU\
**Third-party:** 0.5 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
User-defined

 |

**Operator pods:**\
**IBM:** 0.256 GB RAM\
**Third-party:** 0.2 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
User-defined

 |

**Persistent storage:**\
100 GB

**Ephemeral storage:**\
0.256 GB

**Image storage:**\
Up to 7.91 GB

 |

Minimum resources for an installation with a single replica per service.

Dedicated nodes are recommended. For details, see [Setting up dedicated nodes](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-mgdb/mgdb-dednodes.html).

Development deployment

3 nodes

Production deployment

3 nodes

Recommended configuration

Refer to the [Ops Manager System Requirements](https://www.ibm.com/links?url=https%3A%2F%2Fdocs.opsmanager.mongodb.com%2Fcurrent%2Fcore%2Frequirements%2F%23hardware-requirements "(Opens in a new tab or window)") to determine the appropriate specifications based on your expected workloads.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| OpenPages |

**Operator pods:**\
0.5 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
6 vCPU

 |

**Operator pods:**\
2 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
20 GB RAM

 |

**Persistent storage:**\
252 GB

**Ephemeral storage:**\
10.9 GB

**Image storage:**\
Up to 6.27 GB

 | When you provision the OpenPages service, you specify the size of the instance and the storage class to use. You also specify whether to use the database that is provided with the OpenPages service or a database that is on an external server.

These values represent the minimum resources for OpenPages with a Db2 database on Cloud Pak for Data.

Using a Db2 database on Cloud Pak for Data

OpenPages uses Db2 as a service, which is different from the Db2 service in the services catalog.

You can optionally provision the Db2 database on dedicated nodes. For details, see [Provisioning an instance of OpenPages](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-openpages/openpages-provision.html).

Using a Db2 database outside of Cloud Pak for Data

If you use a database outside of Cloud Pak for Data, the minimum requirements for vCPUs and memory are lower.

 |
| Orchestration Pipelines |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
1.4 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
2.625 GB RAM

 |

**Persistent storage:**\
Uses the persistent storage provisioned by the common core services.

**Ephemeral storage:**\
1.3 GB

**Image storage:**\
Up to 4.31 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| Planning Analytics |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
16 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
28 GB RAM

 |

**Persistent storage:**\
20 GB

**Ephemeral storage:** 50 GB (maximum)

**Image storage:**\
Up to 30.97 GB

 |

Work with IBM Sales to get a more accurate sizing based on your expected workload.

Select the size of your instance when you provision Planning Analytics. For details, see [Provisioning the Planning Analytics service](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-pa/pa-instance.html).

 |
| Product Master |

**Operator pods:**\
0.3 vCPU

**Catalog pods:**\
0.2 vCPU

**Operand:**\
16 vCPU

 |

**Operator pods:**\
0.5 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
34 GB RAM

 |

**Persistent storage:**\
200 GB

**Ephemeral storage:**\
22 GB

**Image storage:**\
Up to 16.86 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| RStudio® Server Runtimes |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
1 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
8.8 GB RAM

 |

**Persistent storage:**\
Uses the persistent storage provisioned by the common core services.

**Ephemeral storage:**This information is not currently available.

**Image storage:**\
Up to 51.30 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| SPSS Modeler |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
0.25 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
1 GB RAM

 |

**Persistent storage:**\
Uses the persistent storage provisioned by the common core services.

**Ephemeral storage:**\
3 GB (maximum)

**Image storage:**\
Up to 9.15 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| Synthetic Data Generator |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
10.15 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
42.5 GB RAM

 |

**Persistent storage:**\
Uses the persistent storage provisioned by the common core services.

**Ephemeral storage:**\
100 GB

**Image storage:**\
Up to 5.76 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| Voice Gateway |

**Operator pods:**\
0.2 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
2 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
8 GB RAM

 |

**Persistent storage:**\
Not applicable

**Ephemeral storage:**\
4 GB

**Image storage:**\
3.54 GB

 |

Minimum resources for a system that can provide voice-only support for up to 11 concurrent calls.

Dedicated nodes are recommended for production environments.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| Watson Discovery |

**Operator pods:**\
0.05 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
15 vCPU

 |

**Operator pods:**\
0.1 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
88 GB RAM

 |

**Persistent storage:**

-   237 GB file storage
-   363 GB block storage
-   215 GB Multicloud Object Gateway storage

**Ephemeral storage:**\
147 GB

**Image storage:**\
Up to 76.95 GB

 | Starter deployments are sized for demonstration purposes only. Production deployments are sized for robust use. Be sure to choose the right size for your needs. You cannot change the deployment type after you install the service. If you need to change it later, you must reinstall. These values represent the minimum requirements for a Starter deployment.

CPUs must support the AVX2 instruction set.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

All of the Watson Discovery service instances associated with an instance of Cloud Pak for Data use the same pool of resources.

Watson Discovery supports only single-zone OpenShift deployments. You cannot install Watson Discovery on a multi-zone deployment.

 |
| Watson Machine Learning |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
6 vCPU

 |

**Operator pods:**\
0.5 GB RAM

**Catalog pods:**\
0.5 GB RAM

**Operand:**\
27 GB RAM

 |

**Persistent storage:**\
150 GB

**Ephemeral storage:**This information is not currently available.

**Image storage:**\
Up to 139.65 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

AVX2 is recommended but not required for AutoAI experiments.

 |
| Watson Machine Learning Accelerator |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
5 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
13 GB RAM

 |

**Persistent storage:**\
73 GB

**Ephemeral storage:**\
2 GB

**Image storage:**\
Up to 26.55 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

The service requires at least one GPU.

GPU support is limited to

-   NVIDIA V100 GPUs
-   NVIDIA A100 GPUs
-   NVIDIA T4 GPUs

 |
| Watson OpenScale |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
13.25 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
68 GB RAM

 |

**Persistent storage:**\
100 GB

**Ephemeral storage:**\
13.5 GB

**Image storage:**\
Up to 35.80 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| Watson Speech services |

**Operator pods:**\
0.3 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
**Speech to Text:** 9 vCPU\
**Text to Speech:** 6.5 vCPU

 |

**Operator pods:**\
0.3 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
**Speech to Text:** 47.7 GB RAM\
**Text to Speech:** 16.4 GB RAM

 |

**Persistent storage:**

-   900 GB
-   20 GB Multicloud Object Gateway storage

**Ephemeral storage:**\
27 GB

**Image storage:**\
Up to 90.39 GB

 |

Minimum resources for an instance with a single replica per service using the default models and voices (US-English). The amount of vCPU, memory, and ephemeral storage that is required increases when you install additional models.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

CPUs must support the AVX2 instruction set.

All of the Watson Speech services service instances associated with an instance of Cloud Pak for Data use the same pool of resources.

 |
| Watson Studio |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
2 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
8.8 GB RAM

 |

**Persistent storage:**\
Uses the persistent storage provisioned by the common core services. Additional storage is required if you enable Visual Studio Code support.

**Ephemeral storage:**\
5 - 10 GB

**Image storage:**\
Up to 6.91 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

If Data Refinery is not installed, add the vCPU and memory required for Data Refinery to the information listed for Watson Studio.

If you enable the Visual Studio Code extension for Watson Studio, you must allocate a minimum of 500-600 MB of storage per user for installed extensions. For details, see *To enable Visual Studio Code* in [Post-installation tasks for the Watson Studio service](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/wsj/install/postinstall-ws.html).

 |
| Watson Studio Runtimes |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
Dictated by the runtimes

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
Dictated by the runtimes

 |

**Persistent storage:**\
Uses the persistent storage provisioned by the common core services.

**Ephemeral storage:**\
Dictated by the runtimes.

**Image storage:**\
Up to 102.41 GB

 | Runtimes use on-demand vCPU and memory.

Watson Studio Runtimes includes the following runtimes:

-   Runtime 24.1 on Python 3.11
-   Runtime 23.1 on Python 3.10
-   Runtime 24.1 on Python 3.11 for GPU
-   Runtime 23.1 on Python 3.10 for GPU
-   Runtime 24.1 on R 4.3
-   Runtime 23.1 on R 4.2

The following runtimes have additional hardware requirements:

Runtime 24.1 on Python 3.11 for GPU

At least 1 GPU core is required to use this runtime.

Runtime 23.1 on Python 3.10 for GPU

At least 1 GPU core is required to use this runtime.

 |
| watsonx.ai |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
27 vCPU

 |

**Operator pods:**\
1 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
665 GB RAM

 |

**Persistent storage:**\
Varies based on the foundation models that you plan to install. For more information, see [Adding foundation models](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-watsonxai/watsonxai-add-models.html).

**Ephemeral storage:**\
Varies based on the foundation models that you plan to install. For more information, see [Adding foundation models](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-watsonxai/watsonxai-add-models.html).

**Image storage:**\
Up to 1.8 TB with all models

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

This service requires GPUs. The number of GPUs depends on the models that you plan to run and whether you plan to run multiple models in parallel. For more information, see [Adding foundation models](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-watsonxai/watsonxai-add-models.html).

GPU support is limited to

-   NVIDIA A100 GPUs with 80 GB RAM
-   NVIDIA H100 GPUs with 80 GB RAM
-   NVIDIA L40S GPUs with 48 GB RAM

    L40S GPUs are not supported for the following foundation models:

    -   granite-20b-multilingual
    -   jais-13b-chat
    -   llama2-13b-dpo-v7
    -   starcoder-15.5b

Restriction: Do not configure NVIDIA Multi-Instance GPU if you plan to install this service.

 |
| watsonx Assistant |

**Operator pods:**\
0.25 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
10 vCPU

 |

**Operator pods:**\
6 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
110 GB RAM

 |

**Persistent storage:**

-   325 GB - 1340 GB

    Only OpenShift Data Foundation and IBM Storage Fusion Data Foundation require 1340 GB of storage. All other storage types require 325 GB.

-   100 GB Multicloud Object Gateway storage

**Ephemeral storage:**\
30 - 135 GB

**Image storage:**\
Up to 61.74 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

All of the watsonx Assistant service instances associated with an instance of Cloud Pak for Data use the same pool of resources.

Your hardware must meet the following additional requirements:

-   CPUs must have a clock speed of 2.4 GHz or higher
-   CPUs must support Linux SSE 4.2
-   CPUs must support the AVX2 instruction set

If you plan to use conversational skills or conversational search features, the service requires a minimum of 2 GPUs for non-HA deployments.

GPU support is limited to

-   NVIDIA A100 GPUs with 80 GB RAM
-   NVIDIA H100 GPUs with 80 GB RAM

Restriction: Do not configure NVIDIA Multi-Instance GPU if you plan to install this service.

 |
| watsonx.data |

**Operator pods:**\
1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
20 vCPU

 |

**Operator pods:**\
0.75 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
62 GB RAM

 |

**Persistent storage:**\
542 GB

**Ephemeral storage:**\
25 GB

**Image storage:**\
Up to 19.91 GB

 |

Minimum resources for an installation with a single replica of the Presto engine.

If you increase the number of Presto replicas, you need additional vCPU, memory, and ephemeral storage.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

If Analytics Engine powered by Apache Spark is not installed, add the vCPU and memory required for Analytics Engine powered by Apache Spark to the information listed for watsonx.data.

 |
| watsonx Code Assistant for Red Hat Ansible® Lightspeed |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
5 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
8 GB RAM

 |

**Persistent storage:**\
25 GB

**Ephemeral storage:**\
0.266 GB

**Image storage:**\
Up to 18.61 GB

 |

Minimum resources for an installation with a single replica per service.

The service requires at least two GPUs.

GPU support is limited to

-   NVIDIA A100 GPUs with 80 GB RAM
-   NVIDIA H100 GPUs with 80 GB RAM
-   NVIDIA L40S GPUs with 48 GB RAM

Restriction: Do not configure NVIDIA Multi-Instance GPU if you plan to install this service.

 |
| watsonx Code Assistant for Z |

**Operator pods:**\
0.1 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
5 vCPU

 |

**Operator pods:**\
0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
8 GB RAM

 |

**Persistent storage:**\
80 GB

**Ephemeral storage:**\
135 MB

**Image storage:**\
Up to 86.93 GB

 |

Minimum resources for an installation with a single replica per service.

The service requires one GPU.

GPU support is limited to

-   NVIDIA A100 GPUs with 80 GB RAM
-   NVIDIA H100 GPUs with 80 GB RAM
-   NVIDIA L40S GPUs with 48 GB RAM

Restriction: Do not configure NVIDIA Multi-Instance GPU if you plan to install this service.

 |
| watsonx.governance |

**Operator pods:**\
0.1 vCPU

-   AI Factsheets: 0.1 vCPU
-   OpenPages: 0.5 vCPU
-   Watson OpenScale: 0.1 vCPU

**Catalog pods:**\
0.01 vCPU

-   AI Factsheets: 0.01 vCPU
-   OpenPages: 0.01 vCPU
-   Watson OpenScale: 0.01 vCPU

**Operand:**

-   AI Factsheets: 0.3 vCPU
-   OpenPages: 6 vCPU
-   Watson OpenScale: 13.25 vCPU

 |

**Operator pods:**\
0.256 GB RAM

-   AI Factsheets: 0.256 GB RAM
-   OpenPages: 2 GB RAM
-   Watson OpenScale: 0.256 GB RAM

**Catalog pods:**\
0.05 GB RAM

-   AI Factsheets: 0.05 GB RAM
-   OpenPages: 0.05 GB RAM
-   Watson OpenScale: 0.05 GB RAM

**Operand:**

-   AI Factsheets: 1.2 GB RAM
-   OpenPages: 20 GB RAM
-   Watson OpenScale: 68 GB RAM

 |

**Persistent storage:**

-   AI Factsheets: Uses the persistent storage provisioned by the common core services.
-   OpenPages: 252 GB
-   Watson OpenScale: 100 GB\
**Ephemeral storage:**\
250 MB

-   AI Factsheets: 300 GB
-   OpenPages: 10.9 GB
-   Watson OpenScale: 13.5 GB

**Image storage:**

-   AI Factsheets: Up to 2.42 GB
-   OpenPages: Up to 6.27 GB
-   Watson OpenScale: Up to 35.80 GB

 |

Minimum resources for an installation with a single replica per service.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

 |
| watsonx Orchestrate |

**Operator pods:**\
0.2 vCPU

**Catalog pods:**\
0.01 vCPU

**Operand:**\
53 vCPU

 |

**Operator pods:**\
0.512 GB RAM

**Catalog pods:**\
0.05 GB RAM

**Operand:**\
293 GB RAM

 |

**Persistent storage:**\
640 GB

**Ephemeral storage:**\
12 GB

**Image storage:**\
Up to 26.36 GB

 |

Minimum resources for a highly available production deployment.

Work with IBM Sales to get a more accurate sizing based on your expected workload.

The service requires a minimum of 2 GPUs for non-HA deployments.

GPU support is limited to

-   NVIDIA A100 GPUs with 80 GB RAM
-   NVIDIA H100 GPUs with 80 GB RAM

Restriction: Do not configure NVIDIA Multi-Instance GPU if you plan to install this service.

 |

* * * * *

* * * * *

IBM Power (ppc64le) hardware

|  |  |
| --- | --- |
|  |  |
|  |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/wsj/analyze-data/pm_service_supported_frameworks.html)

 |
|  |  |
|  |  |

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  |

 |

 |

 |

-   [](https://docs.openshift.com/container-platform/4.12/storage/understanding-ephemeral-storage.html "(Opens in a new tab or window)")
-   [](https://docs.openshift.com/container-platform/4.14/storage/understanding-ephemeral-storage.html "(Opens in a new tab or window)")
-   [](https://docs.openshift.com/container-platform/4.15/storage/understanding-ephemeral-storage.html "(Opens in a new tab or window)")

 |
|  |

 |

 |

 |  |
|  |

 |

 |

 |  |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-db2/aese-dednodes.html)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-dmc/dmc-svc-inst-web.html)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-db2w/db2w-dednodes.html)

 |
|  |

 |

 |

 |  |
|  |

 |

 |

 |  |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/wsj/install/postinstall-ws.html)

 |
|  |

 |

 |

 |  |

* * * * *

* * * * *

Z (s390x) hardware

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/wsj/analyze-data/cp4d-on-ibm-z-features.html)

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  |

 |

 |

 |

-   [](https://docs.openshift.com/container-platform/4.12/storage/understanding-ephemeral-storage.html "(Opens in a new tab or window)")
-   [](https://docs.openshift.com/container-platform/4.14/storage/understanding-ephemeral-storage.html "(Opens in a new tab or window)")
-   [](https://docs.openshift.com/container-platform/4.15/storage/understanding-ephemeral-storage.html "(Opens in a new tab or window)")

 |
|  |

 |

 |

 |  |
|  |

 |

 |

 |  |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-db2/aese-dednodes.html)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-dmc/dmc-svc-inst-web.html)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/svc-db2w/db2w-dednodes.html)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/wsj/install/installing-hadoop-cluster.html)

 |
|  |

 |

 |

 |  |
|  |

 |

 |

 |  |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/wsj/install/postinstall-ws.html)

 |
|  |

 |

 |

 |  |

* * * * *

Automatically installed dependencies[](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware#hardware-reqs__auto__title__1 "Copy to clipboard")
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Automatically installed dependencies provide underlying functionality for services. Use the following sections to understand the hardware requirements for:

-   Common core services
-   Db2 as a service
-   Db2U

Use the following information to determine whether you have the minimum required resources to install each component on your cluster.

* * * * *

x86_64 hardware

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/software-reqs.html#software-reqs__service)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/software-reqs.html#software-reqs__service)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/software-reqs.html#software-reqs__service)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/software-reqs.html#software-reqs__service)

 |

* * * * *

* * * * *

Power (ppc64le) hardware

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/software-reqs.html#software-reqs__service)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/software-reqs.html#software-reqs__service)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/software-reqs.html#software-reqs__service)

 |

* * * * *

* * * * *

Z (s390x) hardware

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/software-reqs.html#software-reqs__service)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/software-reqs.html#software-reqs__service)

 |
|  |

 |

 |

 |

[](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/software-reqs.html#software-reqs__service)

 |

* * * * *

-   **[Downloading the component scaling guidance PDF from the IBM Entitled Registry](https://www.ibm.com/docs/en/SSQNUZ_5.0.x/sys-reqs/downloading-scaling-pdf.html)**\
    Detailed component sizing guidance is available in a PDF file that you can download from the IBM Entitled Registry.
