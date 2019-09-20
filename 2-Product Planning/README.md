# Product Planning
![alt text][group-a-product-planning]

Each team selects top 3 pains/needs from the list as their product roadmap. Put the most valuable and worth to solve problem as the priority one.

The three most common pains mentioned by all groups:

### 1. Difficult to figure out why the IPS blocked (dropped) a flow.

* Can't figure out why certain HTTP flows are getting blocked because of no entries in the block streams table or event logs.
* To rule out false positives, customers want to know:
     * Reputation metadata
     * The logic of Filters
     * Packet/network metadata to what it actually found
     * Meta data for flows that are in the IPS longer than a set threshold
     * Meta data collection for dropped packets that did not match a filter
* With open source IDS (snort) they can see how a filter hits, They could do a trace, but that is expensive because it requires a profile distribution.

### 2. Need IPS performance data to assist with filter tuning.

* Workaround: Automated by custom scripts to run on devices to gather the information / stats that are available on device and to use that to tune the policies
* Graph out Rule stats (can only do that in CLI).
     * Want to chart over time on a per filter basis.
     * Want to know what matches up with bad filter performance.
* Would like to tweak policy and step away and don't have to worry about it. Tweak it based on traffic in network, what policy is catching.

### 3. Better metadata for reputation entries and incident response.

* Want to export it all in one big shot instead of small pieces.
* Having to pull in other tools to figure out what IPS is seeing.
* Want to add more meta data, define own tag and then use it
      * Need more information about why a server is blocked by reputation entry so they can communicate with the owner of the server or their customer as to why it is blocked.
      * Is it everything at an IP address or is it one of many sites at that address?  This type of info is needed.
* Use SPLUNK to pull data into single pane of glass. Helps with response time.
* GoDaddy currently take advantage of msgParameters, but there still isn't enough information to understand why something got blocked.
* Would also like it to be more selective than just IP Address.
* Want to know **why** an IP address got that score.
* GoDaddy can't block anything below 100.

The two most common emerging needs mentioned by all groups:

### 1. Decrypt SSL traffic is needed

* Increased SSL inspection throughput.
      * Want to chart over time on a per filter basis.
      * Increased throughput also requires an equally fast device to process the traffic, i.e. the capacity of the device should not slow down the traffic.
* Ease of HSM Management.
      * Certificates storage and management; interacting with other license management; e.g. AWS interacts with other cert. management
          * e.g. BlueCoat; Both parties need to have traffic going through and have the certificates verified and updated within 5 minutes.
* The group was not pleased when they bought a 40G box and had to pay extra for an SSL license just to have the box inspect traffic at 2G.
* In order for this to be scalable, the SMS has to be able to integrate with an HSM so that once a new certificate is added to the HSM, the SMS can quickly push that certificate to the devices.
     * Otherwise the IPS administrator must get notified a new certificate was added and he must import that onto the SMS and get it pushed to the device.
     * In a customer environment, days, weeks, or months can go by before the cert is added to the SMS and SSL traffic is getting inspected.

### 2. All of your infrastructure are in the cloud

* IPS in the cloud with guaranteed inspection of data
     * Guaranteed delivery path through the IPS; agent on the device or talking to API.
* Flexible cloud solution to meet the needs of regulations or compliance
     * Cloud solution must be flexible enough to meet the regulations, HIPAA, PCI GLB, etc.
* Security stack in every endpoint
     * A way to control egress/ingress in network in the cloud; antivirus; anti-malware.
     * Need the entire security stack baked into every endpoint, servers and VDI, such as HIPS, Anti-Virus, DLP, Endpoint protection

[group-a-product-planning]: https://www.mhlstudio.net/CAB-2018/images/group-a-product-planning.jpg "Group A product planning"
