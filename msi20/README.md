# Integrating Cloud Technologies

## Session Abstract
Tailwind Traders has now migrated the majority of their server hosts from Windows Server 2008 R2 to Windows Server 2019. Now, they are interested in the Azure hybrid technologies that are readily available to them. In this session, learn how Tailwind Traders began using Windows Admin Center to manage its fleet of Windows Server computers and integrated hybrid technologies, such as Azure File Sync, Azure Active Directory Password Protection, Azure Backup, and Windows Defender ATP, to improve deployment performance and manageability.

## Session Story
In this session you’ll demonstrate how Tailwind Traders was able to improve their on-premises environment buy using Azure Hybrid Management services, such as Azure Site Recovery, Azure Update Management and Azure File Sync. You’ll be using the fictional company “Tailwind Traders” as a narrative device. Tailwind Traders represents “everyone”. In this case they’ve on-premises resources and servers, but they face a couple of challenges with server management, like disaster recovery, update management and file servers. They will use the Azure Hybrid services and Windows Admin Center to address these challenges.
<ul>
<li>You will start the session by providing some context about the Tailwind Traders environment and their challenges and that they can address these by using Azure Hybrid services.</li>
<li>You will also show and explain the different hybrid cloud approaches they will use like Azure Stack, Azure Stack HCI and Windows Admin Center</li>
<li>You will then switch to the first Tailwind Traders challenge which is disaster recovery. You will point out their challenges like cost and complexity. You will start demoing how they can address this challenge by using Azure Site Recovery in Windows Admin Center and replicate Hyper-V virtual machines to Azure.</li>
<li>Then you explain what Failover options they now have, like Test Failover, Planned Failover and Failover. You will also point out that you can use this without Windows Admin Center and use Azure Site Recovery also with VMware and physical servers.</li>
<li>The second challenge is management of updates of Linux and Windows virtual machines across on-premise, Azure and other cloud providers. You will show how you can add your Windows Server to Azure Update management using Windows Admin Center. You will also point out that you can do this without Windows Admin Center and include Linux VMs.</li>
<li>You will show how you can assess servers with Update Management and then deploy updates to all your servers to make them compliant.</li>
<li>Another challenge for Tailwind Traders is how they can manage their file servers across different locations efficiently. You will point out the challenges that they have with syncing file servers across different locations and other challenges like space requirements</li>
<li>Then you will show how they can address these challenges with Azure File Sync. You will show how a server syncs up data to an Azure File Share. You will add a second File server and also sync these files across these servers and the Azure File share.</li>
<li>You will finish the presentation by summarize the challenges and how Tailwind Traders solves these by using Azure Hybrid services.</li>
</ul>
By the end of the session you will have taken the audience through some of the most common server challenges customers have today and how Azure hybrid services can help them to overcome these challenges.

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
- [Powerpoint Presentation that includes Speaker Notes](https://globaleventcdn.blob.core.windows.net/assets/msi/msi20/msi20.pptx)
- [Demo/Lab Instructions](https://globaleventcdn.blob.core.windows.net/assets/msi/msi20/MSI20%20LAB%20NOTES-Draft1.docx)
- [Full Length Recording of Presentation](https://globaleventcdn.blob.core.windows.net/assets/msi/msi20/MSI20%20Dry%20Run%203%20Connecting%20Cloud%20Technologies.mp4)
- [Director's Cut of Presentation](https://globaleventcdn.blob.core.windows.net/assets/msi/msi20/MSI20%20Directors%20Cut%20Connecting%20Cloud%20Technologies.mp4)


### Deployment

Almost all sessions can be performed from a trial Azure subscription. Instructions for configuring the subscription with specific assets such as Virtual Machines and resource groups can be found in the Demo/Lab instructions document linked above, often in the form of a script that can be run from Cloud Shell. 

### Demo Videos


- [Azure File Sync](https://globaleventcdn.blob.core.windows.net/assets/msi/msi20/Azure%20File%20Sync.mp4)
- [Network Adapter and WAC Azure Management](https://globaleventcdn.blob.core.windows.net/assets/msi/msi20/Azure%20Network%20Adapter%20and%20WAC%20Azure%20Management%20Mod.mp4)
- [Site Recovery with WAC](https://globaleventcdn.blob.core.windows.net/assets/msi/msi20/Azure%20Site%20Recovery%20with%20WAC.mp4)
- [WAC Azure Update Management](https://globaleventcdn.blob.core.windows.net/assets/msi/msi20/WAC%20Azure%20Update%20Management.mp4)
