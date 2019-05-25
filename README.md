# AWS Well Architected Questions

## Security

SEC 1 -- How do you manage credentials for your workload?	"Credentials include passwords, tokens, and keys that grant access directly or indirectly to manage your workload. Protect credentials with appropriate mechanisms to help you reduce
the risk of accidental or malicious use."
	
SEC 2 -- How do you control human access to services?	"Control human access to services with appropriately defined, limited, and segregated access to help you reduce the risk of unauthorized access."
	
SEC 3 -- How do you control programmatic access to services?	"Control programmatic or automated access to services with appropriately limited short-term credentials and roles to help you reduce the risk of unauthorized access."
	
SEC 4 -- How are you aware of security events in your workload?	"Capture and analyze logs and metrics to gain visibility to security threats and events so that you can take appropriate action."

SEC 5 -- How do you protect your networks?	"Public and private networks and services require multiple layers of defense to help protect your workloads from network-based threats."
	
SEC 6 -- How do you stay up to date with AWS security features and industry security threats?"	"Staying up to date and implementing AWS and industry best practices including services and features can improve the security of your workload. Being aware of the latest security threats will help you build a threat model to identify and implement protective controls."

SEC 7 -- How do you protect your compute resources?	"Configure compute resources with manageable components to protect and monitor their integrity so that you can take appropriate action."

SEC 8 -- How do you classify your data?	"Classification provides a way to categorize data, based on levels of sensitivity, to help you determine appropriate protective controls."
	
SEC 9 -- How do you manage data protection mechanisms?	"Data protection mechanisms include services and keys that protect data in transit and at rest. Protect these services and keys to help you reduce the risk of unauthorized access to systems
and data."
	
SEC 10 -- How do you protect your data at rest?	Protecting your data at rest reduces the risk of unauthorized access or loss.
	
SEC 11 -- How do you protect your data in transit?	Protecting your data in transit reduces the risk of unauthorized access or exposure.
	
SEC 12 -- How do you prepare to respond to an incident?	"Prepare to investigate and respond to security incidents to help you minimize potential disruptions to your workload."
	
## Reliability

REL 1 -- How are you managing AWS service limits for your accounts?	"AWS accounts are provisioned with default service limits to prevent new users from accidentally provisioning more resources than they need. There also limits on how often you can call APIs to protect AWS infrastructure. Evaluate your AWS service needs and request appropriate changes to your limits for each region."
	
REL 2 -- How do you plan your network topology on AWS?	"Applications can exist in one or more environments: EC2-Classic, the default VPC, or VPC(s) created by you. Network considerations such as system connectivity, Elastic IP address and public IP address management, VPC and private address management, and name resolution are fundamental to using resources in the cloud. Well planned and documented deployments are essential to reduce the risk of overlap and contention."
	
REL 3 -- How does your system adapt to changes in demand?	"A scalable system provides elasticity to add and remove resources automatically so that they closely match the current demand at any given point in time."

REL 4 -- How do you monitor AWS resources?	"Logs and metrics are a powerful tool for gaining insight into the health of your workloads. You can configure your system to monitor logs and metrics and send notifications when thresholds are crossed or significant events occur. Ideally, when low-performance thresholds are crossed or failures occur, the system has been architected to automatically self-heal or scale in response."

REL 5 -- How do you implement change?	"Uncontrolled changes to your environment make it difficult to predict the effect of a change. Controlled changes to provisioned AWS resources and workloads are necessary to ensure that the workloads and the operating environment are running known software and can be patched or replaced in a predictable manner."

REL 6 -- How do you back up data?	"Back up data, applications, and operating environments (defined as operating systems
configured with applications) to meet requirements for mean time to recovery (MTTR) and recovery point objectives (RPO)."

REL 7 -- How does your system withstand component failures?	"If your workloads have a requirement, implicit or explicit, for high availability and low mean time to recovery (MTTR), architect your workloads for resiliency and distribute your workloads to withstand outages."
	
REL 8 -- How do you test resilience?	"Test the resilience of your workload to help you find latent bugs that only surface in production. Exercise these tests regularly. "

REL 9 -- How do you plan for disaster recovery?	"Data recovery (DR) is critical should restoration of data be required from backup methods. Your definition of and execution on the objectives, resources, locations, and functions of this data
must align with RTO and RPO objectives."
	
## Performance Efficiency
PERF 1 -- How do you select the best performing architecture?	"Often, multiple approaches are required to get optimal performance across a workload. Well-architected systems use multiple solutions and enable different features to improve
performance"
	
PERF 2 -- How do you select your compute solution?	"The optimal compute solution for a particular system varies based on application design, usage patterns, and configuration settings. Architectures may use different compute solutions for
various components and enable different features to improve performance. Selecting the wrong compute solution for an architecture can lead to lower performance efficiency"
	
PERF 3 -- How do you select your storage solution?	"The optimal storage solution for a system varies based on the kind of access method (block, file, or object), patterns of access (random or sequential), throughput required, frequency of
access (online, offline, archival), frequency of update (WORM, dynamic), and availability and durability constraints. Well-architected systems use multiple storage solutions and enable different features to improve performance."
	
PERF 4 -- How do you select your database solution?	"The optimal database solution for a system varies based on requirements for availability, consistency, partition tolerance, latency, durability, scalability, and query capability. Many systems use different database solutions for various sub-systems and enable different features to improve performance. Selecting the wrong database solution and features for a system can lead to lower performance efficiency."

PERF 5 -- How do you configure your networking solution?	"The optimal network solution for a system varies based on latency, throughput requirements,
and so on. Physical constraints such as user or on-premises resources drive location options,
which can be offset using edge techniques or resource placement."
	
PERF 6 -- How do you evolve your workload to take advantage of new releases?	"When architecting solutions, there is a finite set of options that you can choose from. However,
over time, new technologies and approaches become available that could improve the
performance of your architecture."
	
PERF 7 -- How do you monitor your resources to ensure they are performing as expected?	"System performance can degrade over time. Monitor system performance to identify this degradation and remediate internal or external factors, such as the operating system or application load. "
	
PERF 8 -- How do you use tradeoffs to improve performance?	"When architecting solutions, actively considering tradeoffs enables you to select an optimal approach. Often you can improve performance by trading consistency, durability, and space for time and latency."

## Cost Optimization

COST 1 -- How do you evaluate cost when you select AWS services?	"Amazon EC2, Amazon EBS, and Amazon S3 are building-block AWS services. Managed services, such as Amazon RDS and Amazon DynamoDB, are higher level, or application level, AWS services. By selecting the appropriate building blocks and managed services, you can optimize your architecture for cost. For example, using managed services, you can reduce or remove much of your administrative and operational overhead, freeing you to work on applications and business-related activities."

COST 2 -- How do you meet cost targets with resource type and size choices?	"Ensure that you choose the appropriate AWS resource size for the task at hand. AWS encourages the use of benchmarking assessments to ensure that the type you choose is
optimized for its workload."

COST 3 -- How do you use pricing models to reduce cost?	"Use the pricing model that is most appropriate for your workload to minimize expense. The optimal deployment could be fully On-Demand Instances, a mix of On-Demand and Reserved Instances, or you might include Spot Instances, where applicable."
	
COST 4 -- How do you plan for data transfer charges?	"Ensure that you monitor data transfer charges so that you can make architectural decisions that might alleviate some of these costs. For example, if you are a content provider and have been serving content directly from an S3 bucket to your end users, you might be able to significantly reduce your costs if you push your content to the Amazon CloudFront content delivery network (CDN). Remember that a small yet effective architectural change can drastically reduce your operational costs."

COST 5 -- How do you match supply of resources with customer demand?	"For an architecture that is balanced in terms of spend and performance, ensure that everything you pay for is used and avoid significantly underutilizing instances. A skewed utilization metric in either direction has an adverse impact on your business, in either operational costs (degraded performance due to over-utilization), or wasted AWS expenditures (due to over-provisioning)."
	
COST 6 -- How do you monitor usage and cost?	"Establish policies and procedures to monitor, control, and appropriately assign your costs. Leverage tools provided by AWS for visibility into who is using what, and at what cost. This provides you with a deeper understanding of your business needs and your teams’ operations."

COST 7 -- How do you govern AWS usage?	"Establish policies and mechanisms to make sure that appropriate costs are incurred while objectives are achieved. By employing a checks-and-balances approach through tagging and IAM controls, you can innovate without overspending."
	
COST 8 -- How do you decommission resources?	"Implement change control and resource management from project inception to end-of-life so that you can identify necessary process changes or enhancements where appropriate. Work with AWS Support for recommendations on how to optimize your project for your workload: for example, when to use AWS Auto Scaling, AWS OpsWorks, AWS Data Pipeline, or the different Amazon EC2 provisioning approaches, or review AWS Trusted Advisor cost optimization
recommendations. "
	
COST 9 -- How do you evaluate new services?	"As AWS releases new services and features, it is a best practice to review your existing architectural decisions to ensure they continue to be the most cost effective."
	
## Operational Execellence

OPS 1 -- What factors drive your operational priorities?	"Operational priorities are the focus areas of your operations efforts. Clearly define and agree to your operations priorities to maximize the benefits of your operations efforts."

OPS 2 -- How do you design your workload to enable operability?	"The majority of the lifetime of a workload is typically spent in an operating state. Consider operations needs as a part of system design to help you enable long term sustainment of your workload."
	
OPS 3 -- How do you know that you are ready to support a workload?	"Evaluate the operational readiness of your workload, processes and procedures, and personnel to help you understand the operational risks related to your workload."
	
OPS 4 -- What factors drive your understanding of operational health?	"Define metrics for the evaluation of your workload and processes to help you understand operations effectiveness in supporting business outcomes. Capture and analyze metrics to gainvisibility to processes and events so that you can take appropriate action."
	
OPS 5 -- How do you manage operational events?	"Prepare and validate procedures to respond to operational events to help you minimize their potential disruption to your workload."
	
OPS 6 -- How do you evolve operations?	"Dedicate time and resources for continuous incremental improvement to help evolve theeffectiveness and efficiency of your operations."
