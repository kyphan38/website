# cloud computing

## Essential Characteristics

NIST - 5 characteristics

On demand self-service

- A consumer can unilaterally provision computing capabilities, such as server time and network storage, as needed automatically without requiring human interaction with each service provider
- Can provision capabilities (features and products - VM, storage, databases or networking) as needed without requiring human interaction
- You don't need to inform the vendor days, weeks or months in advance. If you can do this, if you can provision any resource whenever you want, **without involving humans and without delay, it meets this criteria**
- `Provision and terminate using a UI/CLI without human interaction`

Broad network access

- Capabilities are available over the network and accessed through standard mechanisms that promote use by heterogeneous thin or thick client platforms (e.g., mobile phones, tablets, laptops, and workstations)
- Capabilities are available over the **network** and accessed through **standard mechanisms** (HTTP. HTTPS, SSH, Remote Desktop, VPN, etc.)
- `Access services over any networks, on any devices, using standard protocols and methods`

Resource pooling

- The provider’s computing resources are pooled to serve multiple consumers using a multi-tenant model, with different physical and virtual resources dynamically assigned and reassigned according to consumer demand. There is a sense of location independence in that the customer generally has no control or knowledge over the exact location of the provided resources but may be able to specify location at a higher level of abstraction (e.g., country, state, or datacenter). Examples of resources include storage, processing, memory, and network bandwidth
- There is a sense of **location independence** ... no **control** or **knowledge** over the exact **location** of the resources
  - With AWS, you instruct the provider to deploy a virtual machine in a certain region, but they're free to use whatever data centre they want, They're free to use whatever hardware vendor they want
  - IT managers were used to thinking of servers and hardware as their assets. But now, things which host the applications and services, which are the actual things of value to the business
- Resources are **pooled** to serve multiple consumers using a **multi-tenant model**
- `Economies of scale, cheaper service`

Rapid elasticity

- Capabilities can be elastically provisioned and released, in some cases automatically, to scale rapidly outward and inward commensurate with demand. To the consumer, the capabilities available for provisioning often appear to be unlimited and can be appropriated in any quantity at any time
- Capabilities can be e**lastically provisioned** and **released** to scale **rapidly** outward and inward with demand
  - System load increases => system size increases, system load decreases, system reduce in size => Cost of a system will be the same direction with demand
  - Automate the scaling with no human interaction
- To the consumers, the capabilities available for provisioning ofter **appear** to be **unlimited**
- `Scale UP (OUT) and DOWN (IN) automatically in response to system load`

Measured service

- Cloud systems automatically control and optimize resource use by leveraging a metering capability at some level of abstraction appropriate to the type of service (e.g., storage, processing, bandwidth, and active user accounts)Resource usage can be monitored, controlled, and reported, providing transparency for both the provider and consumer of the utilized service
- Resource usage can be **monitored**, **controlled**, **reported** and **BILLED**
  - Pay for that usage
- `Usage is measured. Pay for what you consume`

Table

| Characteristic           | Cloud Computing                                                                                                     | Traditional Computing                                                                                   | Example (Cloud Computing)                                                | Example (Traditional Computing)                                             |
|--------------------------|---------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------|------------------------------------------------------------------------------|
| On-demand self-service    | Provision and terminate using a UI/CLI without human interaction.                                                   | Provisioning requires manual intervention or IT support.                                                 | AWS EC2 instance provisioning                                            | Requesting a new server from the IT department                               |
| Broad network access      | Access services over any networks, on any devices, using standard protocols and methods.                            | Limited to specific network environments or device configurations. Often depends on company infrastructure.| Accessing cloud storage like Google Drive from any device                 | Accessing a local server within a company office only                        |
| Resource pooling          | Resources are pooled to serve multiple consumers using a multi-tenant model. Economies of scale, cheaper service.   | Resources are dedicated to specific users or departments, generally without resource sharing.             | Multiple customers sharing resources in AWS or Azure cloud environments  | Individual physical servers dedicated to departments or applications         |
| Rapid elasticity          | Scale UP (OUT) and DOWN (IN) automatically in response to system load.                                              | Requires manual scaling (additional hardware or IT support).                                             | Automatically scaling instances in Google Cloud when traffic increases  | Manually adding more hardware to a server to accommodate increasing load      |
| Measured service          | Usage is measured. Pay for what you consume.                                                                        | Costs are generally fixed regardless of usage. Resource consumption is not dynamically monitored.        | Pay-per-use model for AWS S3 storage                                     | Paying for a full physical server even if underutilized                       |
