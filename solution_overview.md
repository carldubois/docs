F5 License Deployment Automation
================================

Overview
========

This document describes high-level design recommendations and best practices for
automating the creation, licensing and configuration of virtual F5 BIG-IP
Application Delivery Controllers (ADC). The BIG-IP is load balancer and a full
proxy. It controls the traffic that passes through the public or private data
center network.

Business Value
--------------

The business value for this solution enables the public cloud experience for
internal enterprise cloud infrastructure. It aligns the new F5 purchasing models
with automated workflows.

It eliminates operational bottlenecks, enabling a goal of the Infrastructure as
Code: create an infrastructure definition, an abstracted workflow, that users
consume without additional involvement of IT staff.

The challenge customers face is the complexity of deploying, licensing and
configuring F5 BIG-IP ADCs, limited availability of engineers skilled with F5
BIG-IPs, and the organizational silos within IT operations.

Technical Value
---------------

This solution developed by World Wide Technology, enables the operations
infrastructure team to more rapidly deploy F5 BIG-IP ADCs- increasing the
accuracy of the configuration, saving time and decreasing the wait time for
application developers.

The technical value for the enterprise include these key objectives:

-   *Accelerate* - time-to-delivery

-   *Reduce* - risk of human error

-   *Break down -* IT silos by enabling self-service for the user

Most enterprise application deployments require and benefit from the services
offered by the BIG-IP ADC. The job of provisioning and licensing the BIG-IP is
the responsibility of the data center operations infrastructure team. This is
but one step in the process of moving an application from development, to
testing to production.

Because configuring the BIG-IP ADC is both time consuming and complex,
automating the task reduces the time deploy the application in a production
environment. Every company is now a software company. To compete and survive in
the market, business applications must be developed and available to the
customers at an accelerated pace.

Goals
-----

While this solution focuses on a specific use case, the over-arching goals are
as follows:

-   *Educate* – the customer on the benefits of F5 automation with new
    purchasing models

-   *Demonstrate* - F5 self-service through a uniform push-button user
    experience

-   *Deliver* - a button capable of being consumed by a larger hybrid cloud
    initiative

-   *Inspire* - customers to adopt a DevOps and automation mindset

The F5 License Deployment Automation solution provides one tangible model
supporting these four goals.

F5 License Deployment Automation Components
-------------------------------------------

This solution offered is combined as an Enterprise Agreement (EA) for the
customer. It consists of software licenses, workflow and services as shown in in
the *Solution Component Overview* diagram.

*NOTE: the following diagram will be in-line in the final document*

[Solution Component
Overview](https://wwt.sharepoint.com/sites/F5LicenseDeploymentAutomation/Shared%20Documents/General/solution_reference/images/solution_overview_components_high_level.png)

A description of the individual solution components is as follows:

### Software Licensing

**F5 Licenses**: This solution is bundled and only offered to customers who
purchase F5 licensing through WWT as part of an EA.

**Ansible Licenses**: WWT will bundle the Ansible Tower Premium (100 node
license) with Ansible Engine and Network support as part of the solution.

### Consulting

WWT will provide a fixed number of hours of consulting services and provide
recommendations and guidance for the effective deployment of this solution in
the customer environment. This service may include, but not limited to, Value
Stream Mapping, Agile coaching and an Automation Architect.

The Automation Architect will work with the customer technical staff to remove
any barriers to successfully deploy the solution. They will also provide a
recommendation of staffing and skills needed to operate, troubleshoot and
maintain the solution on a day-to-day basis.

### F5 Automation Workflow

WWT has developed an F5 automation workflow and data model. This workflow
includes a collection of Ansible roles, playbooks and input files package a
solution for developers to easily consume F5 services. The solution includes:

>   Initial provisioning of two Virtual Edition (VE) BIG-IPs into a VMware
>   vCenter

>   Using a BIG-IQ License Manager to license the VE High Availability (HA)
>   BIG-IP pair.

>   Applying the initial configuration to the HA BIG-IP pair, which includes
>   setting the hostname, default password, DNS, SYSLOG, interface and IP
>   addressing, and syncing the configurations.

This workflow may include WWT developed software, open source software and any
modifications to open source software necessary for a functional solution.
Software developed by F5 which is not distributed in the packaged Ansible builds
may also be included.

### Training

Using the ATC portal, customers will be provided self-paced training on the
methods and tools used in the solution. In addition to this Solution Overview
Guide, Installation and Configuration guides and assistance is provided by WWT
resources to deploy the solution in the customer environment.

### Integration Services

This solution includes a demonstration of a simple ServiceNow integration,
demonstrating how to initiate playbooks from ServiceNow, using the Ansible Tower
API. Integration into the ServiceNow instance of the customer can be priced and
provided as part of the EA license.

If a customer desires a custom integration user interface, rather than
ServiceNow, Asynchrony will consult for an additional sales opportunity to
develop an alternative to ServiceNow or the Ansible Tower GUI.

### Maintenance and Support

This solution is comprised of licensed and supported software from Red Hat, F5
Networks and World Wide Technology.

**Ansible by Red Hat:** Supported by licensing Red Hat Ansible Engine and the
Network Automation Add-On bundled with licensing for Ansible Tower Premium. For
more details see: https://www.ansible.com/pricing and
<https://www.ansible.com/ansible-engine> .

**F5 Networks**: Support for F5 products and F5 Ansible modules is provided as
part of the F5 license agreement by contacting F5 Technical Support.

**World Wide Technology**: Support for the WWT provided Ansible roles and
playbooks is provided by WWT as part of the Enterprise Agreement (EA) for this
solution.

*NEED TO REVIEW and UPDATE*

Solution Description
--------------------

This section provides a functional-level description of the F5 license
automation solution.

As a leading value-added reseller focused on integration of solutions from our
industry leading partners, World Wide Technology identifies key customer
operational and organizational challenges and combines technology to address the
business challenges.

The solution is comprised of three layers: Value, Solution and Components.

### Value Layer

The value layer is the operation problem the customer has identified and is
interested in addressing. Value stream mapping techniques, either formerly or
informally, have identified bottlenecks in the current state and designed the
target future state to eliminate the bottleneck.

For this solution, business value is obtained when the DevOps team can
self-provision, license and configure a High Availability pair of Virtual
Edition F5 BIG-IPs into the desired network topology, with the appropriate
service level.

### Solution Layer

The Solution Layer combines software from our leading partners, RedHat and F5
Networks with innovations of WWT to develop the necessary workflow to solve the
business problem of the customer.

The Solution Layer bundles the intellectual property of WWT, along with training
and enablement of the solution in the customer environment. The Solution Layer
is bundled as an Enterprise Agreement (EA) which includes the appropriate
software licenses for the partner components, Ansible Engine and Ansible Tower,
along with software licenses to deploy F5 BIG-IP Virtual Editions.

The Solution Layer orchestrates the workflow through a flexible and modular
design which enables the addition or substitution of various supporting
components.

### Component Layer

The Component Layer are the specific tools and services combined into a workflow
which, when orchestrated by the Solution Layer, create the business value.

The architecture developed by WWT provides a high degree of modularity allowing
customization of the solution to meet a broad range of customer use cases. For
example, Microsoft Teams is shown providing the notification (ChatOps) function
in the *F5 License Automation Solution Components* diagram. However,
substituting Cisco Spark for this function is simply a matter of substituting a
Spark role for the Teams role in the workflow.

The development and licensing of customer specific tools within the Component
Layer can be included in the overall EA agreement.

The three layers are represented in the *F5 License Automation Solution
Components* diagram.

*NOTE: the following diagram will be in-line in the final document*

[F5 License Automation Solution
Components](https://wwt.sharepoint.com/sites/F5LicenseDeploymentAutomation/Shared%20Documents/General/solution_reference/images/solution_overview_components.png)

Solution Benefits
-----------------

The benefits of the F5 License Automation solution include the following:

-   *Public cloud experience* – the solution automates the deployment, licensing
    and provisioning of a High Availability pair of Virtual Edition BIG-IPs in
    an internal cloud environment. Enables on-demand, self-service management of
    licensing for the quick delivery of application services and security to IT
    operations.

-   *Subscription Licensing* - enables organizations to instantiate the VE
    products on demand: Good (LTM), Better (LTM, DNS, AFM, Advanced Routing),
    Best (LTM, DNS, AFM, Advanced Routing, APM, ASM) at data rates from 250 Mbps
    to 10 Gbps

-   *Eliminates day-to-day IT involvement* – IT operations defines the
    environment type through version controlled configuration files, allowing
    the user to provision the environment without manual IT processes.

-   *Role-Based Access Controls* – Role-Based Access Controls (RBAC) are built
    into Tower allowing the user to initiate workflow with maintaining
    confidentiality of the credentials of the underlying infrastructure.
    Credentials are encrypted and only decrypted at the time of workflow
    execution.

-   *Readily Customized* – Workflows can be easily customized due to the modular
    design. The solution is a collection of pre-packaged units of work known to
    Ansible as roles. Roles can be included or removed from the base playbooks
    to tailor the workflow to the environment.

-   *Integration with ServiceNow* – Workflow can be initiated from ServiceNow,
    using the Ansible Tower API to launch jobs.

Technical Assistance
--------------------

Support for this solution is provided by contacting Red Hat and F5 Networks for
the components covered by their respective licenses.

**Contacting Technical Support**

Red Hat Customer Portal -
<https://access.redhat.com/support/contact/technicalSupport>  
Working with F5 Support - <https://f5.com/support/support-policies>

For support questions related to solution components provided by World Wide
Technology, *call insert dave chandler’s home phone here*.

Solution Overview and Best Practices
====================================

This section provides more technical details, including a master architecture
diagram. It provides the technical overview knowledge a WWT CSE needs to
describe the solution to the data center architects.

Deployment Model
----------------

F5 BIG-IPs are commonly deployed in the network topology between the internet
client- a laptop, tablet or mobile device, and the application web server. The
BIG-IP software can be installed on dedicated hardware (BIG-IP or VIPRION
hardware) on as a virtual edition running within a hypervisor.

The BIG-IP is more than a simple load balancer, they can be configured as a full
proxy, providing visibility and control and encryption and decryption of all
traffic passing between the internal and external interfaces.

[INSERT DIAGRAMs showing the workflow this would come from the slides in the
webinar]

Solution Characteristics
------------------------

Table x-x represents the general solution characteristics for F5 License
Automation

-   VMware vCenter Server provides centralized management of vSphere virtual
    infrastructure to host the VE F5 BIG-IPs.

-   An underlay data center network is required with the appropriate port groups
    configured in the vCenter datacenter.

-   Virtual Machine templates (one for each service level) providing a master
    image of the VE F5 BIG-IP.

-   ADD ME

General Best Practices and Guidelines
-------------------------------------

Table x-x presents a list of best practices that have been established through a
combination of design experience, scalability and performance evaluation, and
internal WWT trials.

[NOTE THIS TABLE IS A LIST of THINGS WE LEARNED ALONG THE WAY.

General Solution Caveats
------------------------

Table x-x presents a list of caveats for the solution described in this solution
overview.

[NOTE THIS TABLE IS A LIST of THINGS THAT ARE BROKEN OR MAY BREAK.

Solution Components
===================

This section describes the logical or physical solution components and how it
supports the overall solution.

F5 BIG-IQ License Server
------------------------

TODO NEED A ROLE TO QUERY SERVER AND DESTROY VMS WHICH ARE NO LONGER LICENSED.  
https://www.f5.com/pdf/licensing/big-ip-virtual-edition-subscription-licensing-overview.pdf

F5 Virtual Edition BIG-IP
-------------------------

Ansible Tower
-------------
Joel

VMware vCenter
--------------
Joel

IPAM
----
Joel

Version Control
---------------
Joel

Planning and Design
===================

This section describes why and how the enterprise should consider implementing
this solution. It discusses the user interface, e.g. Ansible Tower GUI,
ServiceNow and how this might interface with the existing workflow. Also
discussed are the roles and responsibilities of the infrastructure operations
staff and the target users – sysadmins and applications developers.

Product Selection
=================

This chapter discusses the systems requirements and software releases evaluated.

### F5 Licensing

*THIS SECTION DESCRIBES THE OPTIONS FOR LICENSING.*  
<https://f5.com/products/how-to-buy/simplified-licensing>

### Ansible Tower

Tower installations can occur in a High Availability (HA) configuration using
two or more nodes. This configuration requires an external–Postgres and MongoDB
installed on a machine that is not one of the primary or secondary tower nodes.

Implementation and Configuration
================================

This chapter provides step-by-step examples of how to implement and configure
the solution.

Installing the Workflow
-----------------------
Tyler
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
For the target customer

/F5-eCLP

cd ACME/roles

ansible-galaxy install --roles-path ./ -r requirements.yml

These directories do not have any .git directorites, and are not .git
repositoriteis. You control what 'branch' is pulled in

from the requirements.yml file

administrator\@russell:/tmp/ACME/roles\$ ls

ansible-f5-addhosts ansible-f5-bigip-sync ansible-f5-include-datamodel
ansible-f5-iworkflow-discover

ansible-f5-bigip-check ansible-f5-create-ha-pair ansible-f5-initial-ha-setup
ansible-f5-iworkflow-onboard

ansible-f5-bigip-import-iapp ansible-f5-create-vs-iworkflow
ansible-f5-iworkflow-cloud-connector ansible-f5-license

ansible-f5-bigip-import-ssl-cert ansible-f5-delete-vm
ansible-f5-iworkflow-cloud-device requirements.yml

administrator\@russell:/tmp/ACME/roles\$

the customer directory has the playbooks and any documentation

administrator\@russell:/tmp/ACME\$ ls

decommission_app.yml decommission_vm.yml deploy.yml files README.md roles
templates

On the public git, create an org (OrangeRetriever)

Create a repo for each of the roles, do not create a readme.

Note: you can also create repos from the API

https://developer.github.com/v3/guides/getting-started/\#create-a-repository

cd ansible-f5-bigip-check

git init

git checkout -b version1

git add \*

git commit -m "first commit"

git remote add origin
https://github.com/OrangeRetriever/ansible-f5-bigip-check.git

git push -u origin version1

alternately create a tar file for the customer

/tmp\$ tar -zcvf /tmp/version1.tgz ./ACME/

tar -ztvf ./version1.tgz
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Data Model Mapping
------------------

Tyler

*TODO: Describe where the YAML files are located and what information need be
obtained from the customer for these files.*

Prepare VMware vCenter Environment
----------------------------------



*TODO: explain what needs be obtained from, and added to vCenter.*

### Configure Resource Group

*TODO: If not configured a resource group will need be created and specified in
the data model.*

### Install OVA Templates

*TODO: Describe what OVA templates need be created.*

### Create Port Groups

*TODO: Port groups for the HA, Internal and External interfaces will need to be
created for each environment.*

Install F5 BIG-IQ License Manager
---------------------------------

*TODO: Describe what needs be done for installing and configuring this machine.*

Installing OS for the Ansible Control Machine
---------------------------------------------

*TODO need guidance on installing Linux: Ubuntu or CentOS/RHEL.*

Installing Ansible Control Machine
----------------------------------

Follow the instructions for installing Ansible to the Control Machine.

[http://docs.ansible.com/ansible/latest/intro_installation.html\#installing-the-control-machine](http://docs.ansible.com/ansible/latest/intro_installation.html%23installing-the-control-machine)

Install Extensions on the Control Machine
-----------------------------------------

*TODO: instructions for running:*  
<https://github.wwt.com/F5-eCLP/ansible-f5-eCLP-tools/blob/version-1.0/deployment/setup_f5_license_automation.yml>

Note: Local extensions are installed in /usr/share/ansible this is the only
modification to the default ansible.cfg file.

Install Ansible Tower
---------------------

Follow the instructions for installing Ansible Tower to the Control Machine.

<http://docs.ansible.com/ansible-tower/latest/html/quickinstall/index.html>

### Update License

*TODO: Explain where to get the license and updated on Ansible Tower.*

### Update Inventory

Use the sample inventory file from
<https://github.wwt.com/F5-eCLP/ansible-f5-eCLP-tools/blob/version-1.0/deployment/inventory.ini>
to configure the inventory file of Ansible Tower.

### Create Credentials

*TODO: Explain what credentials need be created – including Ansible Vault for
the passwords.yml file.*

### Create Project

*TODO: Explain how to create a project for a target customer (e.g. ACME)
repository.*

### Create Job Template

*TODO: Explain now to create the appropriate job templates to execute the
playbooks.*

Diagrams and Configuration Files
================================

*This chapter contains any supplemental diagrams, references and configuration
files not covered in the previous sections. Also contains any appendix
material.*

**Note, this document is modeled after the Cisco CVD document outline:**
<https://www.cisco.com/c/en/us/td/docs/solutions/Enterprise/Video/IPVS/IPVS_DG/IPVS-DesignGuide.pdf>
