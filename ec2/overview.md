# Overview

### Basic Concepts

An EC2 is a VM hosted in AWS. It is the most Popular Offering of Amazon Web Services.&#x20;

* Infrastructure as Service
* Changed based on capacity & usage (Pay as you go)

### Access Keys

Connect using Access keys (SSH key value pairs).&#x20;

It is shown only once.

if lost, create again & old key values will be invalidated

each developer should have their own key pairs

### Security Groups

It is like Firewall.&#x20;

All changes to security groups are instant.

You can have upto 5 security group per instance.&#x20;

**Statefull** :- if a request is sent from an instance, respose is received regardless of inbound rules.&#x20;

### IAM Roles

Can be attached to an instance anytime (running, stopped,etc)

It is the best way for an instance to gain access to other services in AWS

Update to any policy is immediate.&#x20;

### Pricing Options&#x20;

#### On Demand Instance

Can be used any time.

Pay by hour or second

used for unprecidented workload

#### Reserved Instance&#x20;

Used when you know, you need for 1 or more years

usually 1 or 3 years

72% discount

#### Spot Instance&#x20;

90% discount based on auction&#x20;

AWS takes back with less lead time (2 mintues)&#x20;

#### Dedicated Instance&#x20;

BYOL (Bring your own license )

### Instance Data

#### user Data&#x20;

Bootstrap data (like installing softwares like webserver or database)

http://`<ip-address>/latest/userdata`

#### Metadata

get hostname, events, security group

http://`<ip-address>/latest/metadata`

### Network Interface (ENI)

basic interface&#x20;

for high speed, use enhanced network (10-100Gbps)

EFA - Accelatrated High Performace Computing (HPC) and MI

Network interface can be attached

* **warm** : Instance is stopped
* **hot** : instance is running
* **cold** : instance is being launced&#x20;

### Placement groups

Influence AWS to create new instance in a specific AZ

#### Cluster&#x20;

low network latency, high network thoughput

#### Spread

spread across distinct hardwares&#x20;

#### Partition

spread across different logical partition

Typically for hadoop, cassandra and Kafka.

### Spot Fleet

spot can save 90%, collection on spot instance and can have on demand instance also



### Exam Tips

**EC2 Could watch Metrics**&#x20;

* **Default -** CPU, Disk Read/Write, network in or out
* Custom :- Memory

Craete few EC2 instance and get familiar.&#x20;









###

