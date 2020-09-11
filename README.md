# Apache NiFi Prototype

Using Apache NiFi to perform OCR on PDF files.

NiFi is a system of enhancing data through filtering with the help of point source security. It was developed by the National Security Agency to enhance and boost the underlying capacities of the host system NiFi is operating on. NiFi’s main purpose is to automate the data flow between two systems.  This facilitates better flow of data between two systems, one of which is creating data while the other is consuming it. NiFi was formerly called Niagarafiles.

NiFi is built on the philosophy of ensured and guaranteed deliveries. It works by effective load spreading and providing high transaction rates. It supports buffering and can queue the data until the data reaches its intended destination. It also supports prioritized queuing in cases when there are exceptions that the largest, newest or some other data should be processed first. The main goal of NiFi is thus to enhance the data flow between the two underlying systems on which it is running.

## Features

* Guaranteed delivery
* Data buffering with back pressure and pressure release
* Prioritizing queuing
* Flow specifc QoS
* Lineage and Provenance
* Fine-grained history
* Extensable
* Visual command and control
* Clustering

## Abstractions

* FlowFile - an object moving through the system consisting of a byte array and a key/value map.
* FlowFile Processor - software that does a unit of work.
* Connection - linkage between processors.
* Flow Controller - broker facilitating exchange of FlowFiles between processors.
* Process Group - set of processors and connections which has input and output ports.

## Questions

* What is the NiFi CA server?
* How to start Zookeeper with Terraform?
* What is Ranger authentication?
* How are processes checkpointed?
* How are flow versions controlled?
* On the editing window, can there by read-only users?

## Concepts

* Flow Development Life Cycle - FDLC

## Metrics

* Is flow running correctly?
* Number of flow files?
* Size of flow size?
* Size of queues?
* Memory utilization?
* CPU utilization?
* Disk utilization?
* Error counts?


## Links

* Best Links
    * https://nifi.apache.org/
    * https://github.com/apache/nifi
    * https://www.nifi.rocks/
    * https://cwiki.apache.org/confluence/display/NIFI/Apache+NiFi
    * https://pierrevillard.com/best-of-nifi/
* Reference
    * https://linuxadminonline.com/how-to-install-apache-nifi-on-centos-7/
    * https://github.com/jfrazee/awesome-nifi
    * https://stackoverflow.com/questions/tagged/apache-nifi
    * https://medium.com/hashmapinc/creating-custom-processors-and-controllers-in-apache-nifi-e14148740ea
    * https://blog.cloudera.com/?s=nifi
    * https://www.dataintensive.info/
    * https://lonnifi.blogspot.com/
    * https://funnifi.blogspot.com/
    * https://community.cloudera.com/t5/Community-Articles/A-Collection-of-NiFi-Examples/ta-p/244334
* API
    * https://www.rynehanson.com/infosec/nifi-vulnerable-by-design/
* Authentication
    * https://pierrevillard.com/2019/08/21/nifi-with-oidc-using-terraform-on-the-google-cloud-platform
    * https://pierrevillard.com/2017/01/24/integration-of-nifi-with-ldap
    * https://www.thedatanewbie.com/2019/03/how-to-configure-tls-okta.html
* CA
    * https://pierrevillard.com/2019/11/22/secured-nifi-cluster-with-terraform-on-the-google-cloud-platform/
* CI/CD
    * https://medium.com/tech-at-nordstrom/building-ci-cd-pipelines-with-apache-nifi-and-terraform-acedd653b356
* CLI
    * https://dzone.com/articles/devops-tips-using-the-apache-nifi-toolkit-with-apa
* Cluster
    * https://nifi.apache.org/docs/nifi-docs/html/administration-guide.html#clustering
    * https://alvincjin.blogspot.com/search/label/NiFi
    * https://www.nifi.rocks/apache-nifi-docker-compose-cluster/
    * https://dzone.com/articles/modern-apache-nifi-load-balancing
    * https://blogs.apache.org/nifi/entry/load-balancing-across-the-cluster
    * https://pierrevillard.com/2019/11/22/secured-nifi-cluster-with-terraform-on-the-google-cloud-platform/
    * https://pierrevillard.com/2016/11/29/apache-nifi-1-1-0-secured-cluster-setup/
* Docker
    * https://hub.docker.com/r/apache/nifi/
    * https://www.nifi.rocks/official-nifi-docker-image/
    * https://pierrevillard.com/2019/04/09/deploying-nifi-workflows-on-google-cloud-run/
    * https://www.nifi.rocks/apache-nifi-docker-compose-cluster/
* ETL
    * https://github.com/pawl/awesome-etl
* MiNiFi
    * https://nifi.apache.org/minifi/
* Monitoring
    * https://pierrevillard.com/2017/05/15/monitoring-nifi-workflow-sla/
    * https://pierrevillard.com/2017/05/17/monitoring-nifi-scripted-reporting-task/
    * https://www.youtube.com/watch?v=Tt8TSlHu7PE - Back Pressure
* OCR
    * https://www.linkedin.com/pulse/nifi-ocr-using-apache-read-childrens-books-jeremy-dyer/
    * https://github.com/jdye64/nifi-addons
* Python
    * https://github.com/Chaffelson/nipyapi
    * https://github.com/palindromicity/dotifi
    * https://nipyapi.readthedocs.io/en/latest/index.html
    * https://pypi.org/project/nifi-deploy/
* Registry
    * https://pierrevillard.com/2019/07/02/nifi-and-nifi-registry-on-the-google-cloud-platform-with-cloud-source-repositories/
* Rules Engine
    *  https://lonnifi.blogspot.com/
* Scaleability
    * https://blog.cloudera.com/benchmarking-nifi-performance-and-scalability/
* Security
    * https://www.rynehanson.com/infosec/nifi-vulnerable-by-design/
    * https://laconicwolf.com/2018/11/08/examining-code-execution-features-in-apache-nifi/
    * https://medium.com/apache-nifi-security/apache-nifi-sensitive-parameters-vulnerability-f10016aace22
* Terraform
    * https://github.com/chadgeary/nifi
    * https://github.com/Glympse/terraform-provider-nifi
    * https://pierrevillard.com/2019/11/22/secured-nifi-cluster-with-terraform-on-the-google-cloud-platform/
    * https://github.com/Nordstrom/nifi_terraform_generator
* Tips
    * https://pierrevillard.com/2018/07/02/nifi-1-7-terminate-threads/
* TLS
    * https://www.thedatanewbie.com/2019/03/how-to-configure-tls-okta.html
* Training
    * https://www.gologica.com/course/apache-nifi-training/
* Videos
    * https://nifi.apache.org/videos.html
    * https://www.udemy.com/course/apache-nifi-latest-course/
    * https://www.youtube.com/watch?v=fblkgr1PJ0o - Apache NiFi Crash Course
    * https://www.youtube.com/watch?v=VVnFt54jUQ8&list=PL55symSEWBbMBSnNW_Aboh2TpYkNIFMgb - 21 part course
    * https://www.youtube.com/watch?v=9OCNVt4UanA - Hands on Apache NiFi | NiFi Online Training | NiFi Tutorial | Intellipaat
    * https://www.youtube.com/watch?v=VVnFt54jUQ8&list=PL55symSEWBbMBSnNW_Aboh2TpYkNIFMgb - Apache NiFi - the complete guide.
    * https://www.youtube.com/watch?v=sQCgtCoZyFQ - OSCON 2015: Enterprise Dataflow with NiFi.
    * https://www.youtube.com/channel/UCBHGHVGIihzmuOM86D8IfHQ - Steven Koon Channel
    & https://www.youtube.com/watch?v=WX7jrfsWucs - How to ingest files and netflow with NiFi.
    * https://www.youtube.com/watch?v=QPgIv-OJUuk - shows how to use debug processor.
    * https://www.youtube.com/watch?v=RjWstt7nRVY - Apache NiFi Anti-patterns, Part 1
    * https://www.youtube.com/watch?v=v1CoQk730qs - Apache NiFi Anti-patterns, Part 2, Flow Layout
    * https://www.youtube.com/watch?v=rF7FV8cCYIc - Best practicesf rom Renault
    * https://www.youtube.com/watch?v=kK7eVppg9Aw - Storing Apache NiFi Versioned Flows In a Git Repository
    * https://www.youtube.com/watch?v=SZhX_gce63E - Aviation Data Flow
* Documentation
    * https://nifi.apache.org/docs/nifi-docs/
    * https://nifi.apache.org/docs/nifi-registry-docs/

## NiFi People

* Andy LoPresto - @yolopey - member of Apache NiFi PMC
* Bryan Bende - @bbende - member of Apache NiFi PMC
* Mark Payne - @dataflowmark - member of Apache NiFi PMC
* Matt Burgess - @mattyb149 - member of Apache NiFi PMC
* Matt Gilman - @mattgilman - member of Apache NiFi PMC
* Pierre Villard - @pvillard31 - member of Apache NiFi PMC
* Steven Koon - narteck@hotmail.com
* Yolanda M. Davis - yolanda.m.davis@gmail.com
