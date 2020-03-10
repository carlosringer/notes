# Intro to Google Cloud Platform (GCP)

## GCP Structure & Design

### Organization

Projects

- similar to AWS accounts
- own resources
- resources can be shared with other projects
- can be grouped and controlled in a hierarchy

### Compute

Compute Engine (GCE) - Zonal

- virtual machines you can rent, on demand
- Infrastructure as a Service (IaaS)
- similar to Amazons EC2
- boot up on average in 35s
- can customize CPU count and RAM size
- pay by the second (60 sec min) for CPU's, RAM
- cheaper if you keep running it
- even cheaper for "preemptible" or commiting long term usage in a region
- can add GPUs and paid OSes for extra cost

Kubernetes Engine (GKE) - Regional

- managed Kubernetes cluster for running Docker containers with autoscaling
- previously called "Google Container Engine" (but still GKE) until Nov 2017
- released as open source product
- Kubernetes DNS on bu default for service discovery
- no IAM integration (unlike AWS's ECS)
- integrates with persisten disk for storage
- creates GCE instances upon creation
- pay for underlying GCE instances
  - production cluster should have 3+ nodes

App Engine (GAE) - Regional

- Platform as a Service (PaaS) that takes your code and runs it
- similar to elastic beanstalk and heroku
- more that just compute
- flex mode ("App Engine Flex") can run any container, any language
- auto scales based on load
  - will turn off the last instance if you get no traffic
- pay for underlying GCE instances

Cloud Functions (GCF)

- runs node.js code in response to an event
- can make shims for different languages
- Functions as a service (FaaS), "Serverless"
- similar to AWS lambda functions
- pay for CPU and RAM assigned to function per 100ms (min 100ms)
  - only pay when function is ran
- each function automatically gets an HTTP endpoint
- can be triggered by GCS objects, pub/sub messages, etc
- massively scalable (horizontally)

## Storage, Database, & Transfer

Local SSD - Zonal

- very fast 375GB solid state drives physically attached to the server
- similar to EC2 instance stored volumes and direct-attached storage (DAS) on local computer
- attached tp single GCE storage instance
- offer incredibly high performance
- data will be lost whenever the instance shits down (on purpose or not)
  - but can survive a Live Migration
- like all data at rest with Google, always encrypted
- pay by GB-month provisioned (prorated)

Persistent Disk (PD) - Zonal

- flexible, block-based network-attached storage; boot disk for every GCE instance
- compares to Elastic Block Storage (EBS) or storage area network (SAN)
- larger the volume faster the drives get
  - performance scales with volume size; max way below Local SSD, but still fast
- persistent disks persist, and are replicated for durability
- can resize while in use (up to 10TB), but will need file system update within VM
- snapshots (and machine images) add even more capability and flexibility
  - pay for incremental ($ and time), but use/delete like full backups
- not file- based NAS, but can mount to multiple instansces if all are read-only
- pay for GB/mo provisioned depending on perf. class; plus snapshot GB/mp used

Cloud SQL - Regional
