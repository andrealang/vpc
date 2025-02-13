---

copyright:
  years: 2018, 2021
lastupdated: "2021-03-02"

keywords: virtual server instances, VSI, compute, virtual machines, planning, best practices, instances, virtual servers, virtual server instance, Virtual servers for VPC, gen 2, generation 2, infrastructure, infrastructure as a service, IaaS

subcollection: vpc

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:deprecated: .deprecated}
{:external: target="_blank" .external}
{:table: .aria-labeledby="caption"}

# About virtual server instances for VPC
{: #about-advanced-virtual-servers}

Virtual servers for VPC is an Infrastructure-as-a-Service (IaaS) offering that gives you access to all of the benefits of {{site.data.keyword.vpc_short}}, including network isolation, security, and flexibility. 

With virtual server instances for VPC, you can quickly provision instances with high network performance. When you provision an instance, you select a profile that matches the amount of memory and compute power that you need for the application that you plan to run on the instance. Instances are available on the x86 architecture. After you provision an instance, you control and manage those infrastructure resources. 
{: shortdesc}

## How are virtual server instances for VPC different from other IBM virtual server offerings?
{: #how-are-vsis-different}

In the IBM Cloud Virtual Server for Classic infrastructure offering, instances use native subnet and VLAN networking to communicate to each other within a data center (and single pod). Using subnet and VLAN networking in one pod works well until you must scale up or have large virtual resource demands that require resources to be created between pods. (Adding appliances for VLAN spanning can get expensive and complicated!) 

{{site.data.keyword.vpc_short}} adds a network orchestration layer that eliminates the pod boundary, creating increased capacity for scaling instances. The network orchestration layer handles all of the networking for all virtual server instances that are within a VPC across regions and zones. With the software defined networking capabilities that VPC provides, you have more options for multi-vNIC instances and larger subnet sizes. 

To review and start deploying compute resources, see the following topics:

|              Deployment options                           |  Description                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
|[Virtual Servers for VPC profiles](/docs/vpc?topic=vpc-profiles#profiles) | IBM Cloud Virtual Servers for VPC provide the advanced security of a private cloud with the agility and ease of a public cloud. Virtual servers for VPC offer the best network performance (up to 80 Gbps), best security, and fastest provisioning times.|
|[Dedicated hosts for VPC](/docs/vpc?topic=vpc-creating-dedicated-hosts-instances) | With dedicated host availability, you can choose to create a single-tenancy environment where you can provision virtual server instances according to your needs.|
|[Virtual Servers for Classic](/docs/virtual-servers?topic=virtual-servers-getting-started-tutorial)| When you create an x86-based virtual server in classic infrastructure, you have a lot of options. You can choose between a public (multi-tenancy) environment or a dedicated (single-tenancy) environment. Then, depending on the chosen environment, you select hourly, monthly, or transient virtual servers. In the case of public virtual servers, you also choose to use either SAN-based storage or local storage. |
{: caption="Table 1. Deployment options" caption-side="top"}   

To compare all virtual compute options, see [Compare Virtual Compute options](https://www.ibm.com/cloud/virtual-servers/options){: external}.

## Creating virtual servers for VPC

To continue by creating virtual servers for VPC, see the following topics:

|              Provisioning instructions                          |  Description                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
| [Planning for instances](/docs/vpc?topic=vpc-vsi_best_practices) | This configuration checklist is helpful to get the most out of your {{site.data.keyword.vpc_short}} deployment. | 
|[Creating virtual server instances by using the UI](/docs/vpc?topic=vpc-creating-virtual-servers) | Provision public instances with various options by using the user interface.|
|[Creating virtual server instances by using the CLI](/docs/vpc?topic=vpc-creating-virtual-servers-cli)| Provision public instances with various options by using the command line interface. |
| [Creating an instance by using the API](/docs/vpc?topic=vpc-creating-a-vpc-using-the-rest-apis#select-profile-and-image)| Provision public instances with various options by using the API. |
|[Creating instances on dedicated hosts](/docs/vpc?topic=vpc-creating-instance-on-dh)| Provision instances on a dedicated host or group. |
{: caption="Table 2. Links to provisioning instructions" caption-side="top"}  


