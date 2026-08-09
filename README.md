# SAP-BW-Bridge
This document introduces SAP BW Bridge and describes how it can be used to migrate SAP BW data and models to SAP Datasphere, as well as how to archive BW data without it.

## 1. Migrate SAP BW to SAP Datasphere
To help customers leverage their existing investment in SAP BW, SAP provides transition tools to  migrate BW objects into BW-Bridge.

![alt text](/images/BW_Migration_1.png)

**BW Tools**: InfoProviders(BW) -> ADSOs(BW-Bridge) -> Tables/Views/Models(Datasphere)

> [!NOTE]
> Bex Query design is converted in BW-Bridge. But it cannot be executed.

Good[blog](https://community.sap.com/t5/technology-blog-posts-by-sap/how-to-migrate-data-from-sap-bw-to-sap-datasphere-bw-bridge-or-sap-bw-4hana/ba-p/13668426?utm_source=chatgpt.com)

## 2. Create BW-Bridge
- Allocate Resource

![alt text](/images/BW_Bridge_1.png)

- Create BW Instance and BW Bridge Space

![alt text](/images/BW_Bridge_2.png)

# 3. Archive BW Data without BW Bridge

If the goal is to archive SAP BW data, you can create an **Open Hub** on an InfoProvider and use a SAP Datasphere Replication Flow to consume the data through **ODP** (Open Hub BW Extractor) and load it into SAP **HANA Data Lake** storage.


 
