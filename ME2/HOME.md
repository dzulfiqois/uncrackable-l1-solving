# Installation Guide ‐ Mata Elang v2

## Overview

Snort is a well-known, signature-based network intrusion detection system (NIDS). The Snort sensor must be placed within the same physical network, and the defense centers in the typical NIDS architecture offer limited network coverage, especially for remote networks with a restricted bandwidth and network policy. Additionally, the growing number of sensor instances, followed by a quick increase in log data volume, has caused the present system to face big data challenges. This research paper proposes a novel design for a cloud-based Snort NIDS using containers and implementing big data in the defense center to overcome these problems. Our design consists of Docker as the sensor’s platform, Apache Kafka as the distributed messaging system, and big data technology orchestrated on lambda architecture. We conducted experiments to measure sensor deployment, optimum message delivery from the sensors to the defense center, aggregation speed, and efficiency in the data-processing performance of the defense center. We successfully developed a cloud-based Snort NIDS and found the optimum method for message delivery from the sensor to the defense center. We also succeeded in developing the dashboard and attack maps to display the attack statistics and visualize the attacks. Our first design is reported to implement the big data architecture, namely, lambda architecture, as the defense center and utilize rapid deployment of Snort NIDS using Docker technology as the network security monitoring platform.

Mata Elang is the evolution of the Mata Garuda Internet Monitoring Project for Indonesia. This project was initialized as a private repository in 2018 by LabJarkomC307 - Politeknik Elektronika Negeri Surabaya. Currently, Mata Elang is a collaboration research between PENS, Universitas Indonesia, and BRIN (Badan Riset dan Inovasi Nasional). Mata Elang is supported by JICA.

This project is based on the article :
Saputra, F.A.; Salman, M.; Hasim, J.A.N.; Nadhori, I.U.; Ramli, K. The Next-Generation NIDS Platform: Cloud-Based Snort NIDS Using Containers and Big Data. Big Data Cogn. Comput. 2022, 6, 19. https://doi.org/10.3390/bdcc6010019

![Mata Elang](https://user-images.githubusercontent.com/11935643/214498807-0b07f8a2-5cb8-406f-8e85-4bcb7a6e3d7f.png)

## Installation

Here, as an example, we will show you how to set up the Mata Elang Platform.

<!-- #### All Servers

1. [Time Zone and NTP](/mata-elang-stable/mataelang-platform/wiki/time-zone-and-ntp) -->

#### Sensor Installation and Configuration

1. [Sensor](/ME2/Installation-and-Configuration.md#setting-up-for-sensor)

#### Defense Center Installation and Configuration

2. [Defense Center Installation](/ME2/Installation-and-Configuration.md#setting-up-for-defense-center)
   <!-- 3. [Mosquitto](/mata-elang-stable/mataelang-platform/wiki/mosquitto) -->
   <!-- 4. [Hadoop](/mata-elang-stable/mataelang-platform/wiki/hadoop) -->
   <!-- 5. [Kafka](/mata-elang-stable/mataelang-platform/wiki/kafka) -->
   <!-- 6. [Spark & KaspaCore](/mata-elang-stable/mataelang-platform/wiki/spark-&-kaspacore) -->
   <!-- 7. [OpenSearch](/mata-elang-stable/mataelang-platform/wiki/opensearch) -->
   <!-- 8. [Zabbix](/mata-elang-stable/mataelang-platform/wiki/zabbix) -->

<!-- ## Configurations -->

<!-- - [Configurations](/Mata-Elang-Stable/MataElang-Platform/wiki/configurations) -->

## Operation and Maintenance

- [Startup/Shutdown Procedures]()
- User Management

  - [OpenSearch](/mata-elang-stable/MataElang-Platform/wiki/OpenSearch-User-Account-Management)

- Sensor Management
  - [Update Sensor Rule](/mata-elang-stable/sensor-snort#configure-snort-rule-auto-update-optional)
  - [Capture Sensor Log and Change Log Limit Size](/mata-elang-stable/sensor-snort#get-pcap-files)
  - [Security Consideration](/mata-elang-stable/MataElang-Platform/wiki/Snort#warning-warning-warning)
- [Backup](/mata-elang-stable/mataelang-docs/blob/main/BACKUP.md)
- [Update Software Version](/mata-elang-stable/MataElang-Platform/wiki/Update-Software-Version)
- [Troubleshooting](/mata-elang-stable/mataelang-platform/wiki/troubleshooting)

## Offline Installation

- [Offline Installation]()
- [How to make offline installation media]()
