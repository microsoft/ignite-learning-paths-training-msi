# MSI10: Migrating to Windows Server 2019

![Learning Path](https://img.shields.io/badge/Learning%20Path-MSI-fe5e00?logo=microsoft)

## Session Abstract
Tailwind Traders has acquired Northwind, a large subsidiary company. Northwind currently has 1500 servers running Windows Server 2008 R2 - either directly or virtually - on hardware at the midpoint of its operational lifespan. While Tailwind Traders will eventually move many of these workloads to Azure, Windows Server 2008 R2 end of life is quickly approaching. In this session, learn how Tailwind Traders’ used Azure hybrid management technologies to migrate servers, and the roles that they host, to Windows Server 2019.

## Session Story
In this session you will demonstrate how Tailwind Traders was confronted with the reality of their core infrastructure services on premises is running on Windows 2008 R2 and as such in a dangerous state with regards to End of Support. What this means is Their most critical source of Identity – Active Directory – will become more and more vulnerable the longer it runs without security updates. Because it is one of the core workloads the CANNOT be migrated to the cloud wholeheartedly, a systemic and complete migration of all their domain controller infrastructure is required. The Tailwind Traders company has 30+ sites around the world and has a representative breakdown of at least one DC, a series of App servers, DHCP servers and File Servers that need to be updated OR migrated to Azure in order to mitigate future security update issues.

Tailwind Traders are in a situation not unlike the MAJORITY of our customers who are explore more Azure usage. While new workloads and certain existing on-prem workloads can migrate and evolve / modernize in Azure – these core services (AD, App, DHCP, DNS, FileServer) represent the majority of Windows Server 2008 R2 servers in the marketplace.
<ul>
<li>You start the session working through the main issue that should drive updates of the OS – End of Support (meaning no more patches or security updates & no phone support). This could very well result in the loss of certification & compliance for a number of major verticals. One solution is to migrate compatible workloads to Azure IaaS or PaaS services, but this will take time and only certain workloads can fit this model. We present a logical flow for making these decisions as a member of the planning team.</li>
<li>The first demo relates to any number of ways you can querry and discover Windows Server based workloads. We opt for a simple Active Directory querry using Active Directory Admin Center as well as PowerShell – something that is free to all Microsoft customers. After identifying the main systems that need to be migrated to a more modern Windows Server version – we make a list and plan an attack on how to migrate these workloads.</li> 
<li>The more intricate / manual process affecting the “biggest hit” for this migration is to target the Active Directory domain controller infrastructure. This process of migration involves promoting a 2019 member server to a domain controller, transferring FSMO roles and demoting the old domain controller. This would normally proceed to all 30 sites, but for this demo environment – we only focus on the mechanics of completing one site. With the exception of the DCPROMO process on the 2008R2 server – everything is done via command line and PowerShell.</li>
<li>After the domain controllers have been migrated –  you focus on the primary infrastructure services including DHCP. In this demo, there are manual reservations as well as active clients using the DHCP leases. We use the same Server Migration Tools that were introduced in 2012, and updated with each version of Windows Server released to production. In this instance we also migrate the IP address from the old system to minimize client interruption with DHCP lease renewal.</li>
<li>The most popular role old Windows Server 2008R2 systems have after Domain Controllers is the role of a FileServer. These systems are usually front ends for SAN storage or possibly clustered for availability. File servers hold the wealth of knowledge within a company that has spanned decades of information management. You will be using the new and updated Storage Migration Service which is deployed and managed through Windows Admin Center. This system can now migrate file servers and File Server Clusters from 2003 R2 up to 2019 including Linux SAMBA boxes and dedicated SAN / NAS boxes. This demo is very impactful due to the simplification of the complexity involved in transferring users, groups, file permissions, storage and mapping to new systems as well as assuming the identity of old systems to minimize client impact.</li> 
</ul>
At the end of each demo – there are links to documents and resources that should be use by attendees in order to start their journey in learning how to migrate these critical workloads to a more modern and Hybrid capable Windows Server 2019. This content will evolve as Microsoft Ignite the tour progresses as there are a number of migration helpers coming out for Windows Admin Center. 

## How to use this repository
Welcome, Presenter!

We're glad you are here and look forward to your delivery of this content.

As an experienced presenter, we know you know HOW to present so this guide will focus on WHAT you need to present.

Among many resources, a full run-through video of the presentation, delivered by the original content creator is available to review and a great starting point. A director's cut edition, with additional information from the original content creator, is also available for review.

Along with the video of the presentation, this document will link to all the assets you need to successfully present including PowerPoint slides, demo videos, and demo instructions.

Read this document in its entirety. Watch the video presentation(s), review and practice with the demo videos and have a fantastically successful time presenting this content.

Ask questions of the Lead Presenter and trained speakers (list below).

## Getting Started
These instructions consist of the steps you should go through in preparing to present this content:

### Assets in the Train-the-Trainer Kit


- This guide
- [Powerpoint Presentation that includes Speaker Notes](https://globaleventcdn.blob.core.windows.net/assets/msi/msi10/msi10.pptx)
- [Demo/Lab Instructions](#)
- [Full Length Recording of Presentation](https://globaleventcdn.blob.core.windows.net/assets/msi/msi10/msi10-Migrating%20to%202019%20-%20v2.mp4)
- [Director's Cut of Presentation](#)
- [Ignite 2019 Session Presentation](https://globaleventcdn.blob.core.windows.net/assets/msi/msi10/MSI_10_IGNITE.mp4)


### Deployment

Almost all sessions can be performed from a trial Azure subscription. This session is a little different in that it all occurs using "on premesis" assets, specifically Windows Server virtual machines running either Windows Server 2008 R2 or Windows Server 2019. Instructions on how to build the lab will be provided at a future point in time. 

### Demo Videos


- [Demo 1: Server Discovery](https://globaleventcdn.blob.core.windows.net/assets/msi/msi10/MSI-10-Demo-1-Discovery.mp4)
- [Demo 2: DC Promotion and FSMO Migration](https://globaleventcdn.blob.core.windows.net/assets/msi/msi10/MSI-10-Demo-2-DCPromoFSMO.mp4)
- [Demo 3: DHCP Migration](https://globaleventcdn.blob.core.windows.net/assets/msi/msi10/MSI-10-Demo-3-dhcp-migration-msi10.mp4)
- [Demo 4: Storage Migration Services](https://globaleventcdn.blob.core.windows.net/assets/msi/msi10/MSI-10-Demo-4-Edit.mp4)

