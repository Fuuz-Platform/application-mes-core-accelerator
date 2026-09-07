# application-mes-core-accelerator

> **Fuuz Industrial Operations Platform — Manufacturing Execution System (Core)**
> Package Version: `1.0.0` | Platform Version: `2025.11.3` | Spec: `2.0.0`

The **MES Core** accelerator is the foundational Manufacturing Execution System package built on the [Fuuz Industrial Operations Platform](https://fuuz.com). It provides the complete module registry, platform-level data architecture, and core operational workflows that underpin discrete and process manufacturing execution. This package establishes the full organizational and functional hierarchy used across all Fuuz MES accelerators, making it the essential baseline for any manufacturing deployment.

This package contains **41 modules** across **18 functional areas**, **32 data flows**, **92 data models**, **56 screens**, and **34 seed data records**.

---

## Table of Contents

1. [Overview](#overview)
2. [Module Structure](#module-structure)
3. [Functional Areas](#functional-areas)
4. [Data Flows](#data-flows)
5. [Data Models](#data-models)
6. [Screens](#screens)
7. [Access Control](#access-control)
8. [Package Contents](#package-contents)
9. [Dependencies](#dependencies)
10. [Installation](#installation)

---

## Overview

The MES Core accelerator provides the foundational infrastructure for manufacturing operations management, including:

- **Platform Module Registry** — The complete set of module group and module definitions that organize all Fuuz MES functionality into a structured, navigable hierarchy
- **Production Management** — Work order management, advanced production scheduling, Kanban production, planning, and manufacturing execution
- **Shop Floor Execution** — Control panels (work center operator terminals), Andon/request management, and real-time production monitoring
- **Resource Management** — Workunits (equipment/work center state tracking), resource assignment, and availability management
- **Quality Control** — Quality data models and specifications integrated with production workflows
- **Materials Management** — Inventory tracking, storage management, logistics, and material staging
- **Traceability and Genealogy** — Full genealogy tracking across production orders and material movements
- **Warehouse Management** — Inventory control, location management, and warehouse operations foundation
- **System Platform** — Access control, configuration management, scheduling engine, orchestration, IoT integration, integration framework, data modeling, business intelligence, and application lifecycle management
- **Product Data Management** — Engineering data, materials specifications, and quality specifications
- **Supply Chain Management** — Procurement and supplier management workflows
- **Human Capital Management** — Employee records and workforce data
- **Customer Relationship Management** — Customer and sales management
- **Documentation** — Confluence-based documentation integration
- **EDI** — Electronic data interchange foundation

---

## Module Structure

| Module Group | Modules |
|---|---|
| **Applications** | Application Connector, Application Lifecycle Management, Application Trace |
| **Customer Relationship Management** | Sales |
| **Documentation** | Confluence |
| **EDI** | *(EDI foundation)* |
| **Human Capital Management** | Employees |
| **Maintenance Management** | Maintenance |
| **Materials Management** | Inventory, Logistics, Storage Management |
| **Mobile** | *(Mobile foundation)* |
| **Product Data Management** | Engineering, Materials, Quality |
| **Production Management** | Advanced Production Scheduling, Customer Management, Kanban Production, Manufacturing, Planning, Product Data Management, Supplier Management, Work Order Management |
| **Quality Control** | *(Quality foundation)* |
| **Reporting and Analytics** | Business Intelligence |
| **Resource Management** | Resources, Workunits |
| **Shop Floor Execution** | Control Panels, Request Management |
| **Supply Chain Management** | Procurement |
| **System** | Access Control, Application Setup, Configuration, Dashboard, Data Management, Data Modeling, Files, Integration, Integration (NetSuite), Internet of Things, Orchestration, Scheduling, Testing |
| **Traceability and Genealogy** | Genealogy Tracking |
| **Warehouse Management** | Inventory Control |

---

## Functional Areas

### Production Management

Core production execution and scheduling infrastructure:

- **Work Order Management** — Create, dispatch, track, and close manufacturing work orders; capture actual vs. planned quantities, cycle times, and completion status
- **Advanced Production Scheduling** — Constraint-based forward/backward scheduling with capacity visibility and scheduling board integration
- **Kanban Production** — Pull-based Kanban card management with configurable replenishment triggers and signal workflows
- **Planning** — Production planning workflows with demand-driven order generation
- **Manufacturing** — Core manufacturing execution with operation-level tracking, time capture, and status management
- **Customer Management** — Customer-facing production data and order-linked manufacturing workflows
- **Supplier Management** — Supplier-linked production inputs and incoming material tracking

### Shop Floor Execution

Operator-level production control and communication:

- **Control Panels** — Work center operator terminals providing real-time visibility into active production orders, operation instructions, production count recording, and labor capture
- **Request Management (Andon)** — Structured shop floor request and escalation system for downtime events, material shortages, quality holds, and maintenance requests; configurable response workflows with notification routing

### Resource Management

Equipment and work center availability tracking:

- **Workunits** — Real-time work center and equipment state management (running, idle, down, maintenance); automated state history tracking with end-date backfill and duration calculation; the core data engine powering OEE and utilization reporting
- **Resources** — Resource registry with capability classification, assignment to work orders, and availability scheduling

### Materials Management

Inventory, storage, and logistics operations:

- **Inventory** — Real-time inventory balance tracking by location, lot, and serial number with transaction history
- **Storage Management** — Location hierarchy management, bin/rack/shelf assignment, and storage rule configuration
- **Logistics** — Material movement workflows including transfers, staging for production, and inter-facility logistics

### Product Data Management

Engineering and specification management:

- **Engineering** — Engineering change management, revision control, and released engineering data linked to production workflows
- **Materials** — Material master data including specifications, approved supplier lists, and procurement parameters
- **Quality** — Quality specification management linked to inspection plans and in-process check criteria

### Traceability and Genealogy

Material and production traceability:

- **Genealogy Tracking** — Forward and backward genealogy across lots, serials, and work orders; component-to-assembly lineage; trace queries for compliance, recalls, and customer investigations

### Warehouse Management

Foundational warehouse operations:

- **Inventory Control** — Cycle count management, inventory adjustment workflows, ABC classification, and reorder point management

### System Platform

Core platform infrastructure and administration:

- **Access Control** — Role-based access management, permission assignment, and user provisioning workflows
- **Configuration** — System-wide settings management including reason codes, unit-of-measure tables, lookup tables, and configurable parameters
- **Scheduling** — Background job scheduling engine for automated flow execution, report generation, and maintenance triggers
- **Orchestration** — Multi-step workflow orchestration for complex cross-module business processes
- **Internet of Things (IoT)** — Device registry, tag mapping, and real-time data ingestion from PLCs, sensors, and SCADA systems
- **Integration** — Generic integration framework for external system connectivity with configurable mapping and transformation
- **Integration (NetSuite)** — Pre-built NetSuite ERP connector for bidirectional work order, inventory, and transaction synchronization
- **Data Modeling** — Platform-level data model management and schema configuration
- **Data Management** — Data import/export, bulk operations, and data governance workflows
- **Business Intelligence** — Configurable analytics and reporting infrastructure with dashboard builder
- **Dashboard** — System dashboard framework with widget-based layout and KPI display
- **Files** — File attachment management for documents, images, and binary assets across all platform entities
- **Application Setup** — Initial platform configuration, tenant setup, and deployment initialization workflows
- **Application Lifecycle Management** — Package versioning, deployment, and environment promotion workflows
- **Application Connector** — Cross-application integration and service connector framework
- **Application Trace** — Audit logging, flow execution tracing, and operational diagnostics
- **Testing** — Automated testing framework for flow validation and platform regression testing

### Supply Chain Management

Procurement and supplier operations:

- **Procurement** — Purchase order management, receiving integration, supplier performance tracking, and procurement approval workflows

### Human Capital Management

Workforce data foundation:

- **Employees** — Employee records, skill profiles, certification tracking, and workforce organizational hierarchy

### Customer Relationship Management

Customer data and sales operations:

- **Sales** — Customer order management, sales order–to–work order linking, and customer communication workflows

### Maintenance Management

Asset and maintenance foundation:

- **Maintenance** — Maintenance work order framework, asset registry integration, and downtime capture linked to workunit state management

---

## Data Flows

The package includes **32 data flow files** providing core platform automation:

| Flow Type | Examples |
|---|---|
| **System (Scheduled)** | Workunit state history end-date backfill and duration calculation; scheduled data maintenance and cleanup operations |
| **System (Background)** | Work order status transitions; inventory balance recalculation; Kanban signal processing |
| **Screen** | UI-driven flows for production recording, work order operations, inventory transactions, and request submission |
| **Integration** | NetSuite ERP sync flows; IoT device data ingestion; external system webhook processing |

Flow types used across the package:
- **System** — Backend/scheduled business logic, data processing pipelines, and automated state management
- **Screen** — User-interface-triggered flows responding to form submissions and operator actions
- **Integration** — External system connectors with bidirectional data synchronization

### Notable Data Flows

- **Back Fill End Dates of Workunit History** — Scheduled system flow that identifies workunit state history records with null `endAt` values, calculates durations using JSONata groupBy and map operations, and performs bulk GraphQL mutations to maintain accurate availability and OEE history data
- **Kanban Production Signals** — Automated Kanban card replenishment trigger processing with configurable min/max thresholds
- **Work Order Status Transitions** — Orchestrated workflow managing work order lifecycle state changes with validation and downstream notifications
- **NetSuite Integration Sync** — Bidirectional synchronization of production orders, inventory transactions, and BOM data with Oracle NetSuite ERP

---

## Data Models

The package includes **92 data model files** covering all foundational platform entities:

**Production** — WorkOrder, WorkOrderOperation, ProductionRecord, WorkCenter, WorkCenterCapacity, KanbanCard, ProductionSchedule

**Resources** — Workunit, WorkunitState, WorkunitStateHistory, Resource, ResourceCapability, ResourceAssignment

**Quality** — QualitySpecification, InspectionCriteria, QualityCheck, NonConformanceRecord

**Materials** — Inventory, InventoryLocation, InventoryTransaction, Lot, Serial, MaterialMaster, StorageLocation

**Genealogy** — GenealogyRecord, ComponentTrace, MaterialTrace, ProductionLineage

**Warehouse** — CycleCount, CycleCountLine, InventoryAdjustment

**Procurement** — PurchaseOrder, PurchaseOrderLine, Supplier, SupplierPerformance

**Engineering** — EngineeringChange, BOMRevision, MaterialSpecification

**Maintenance** — MaintenanceWorkOrder, Asset, DowntimeEvent

**Labor** — Employee, OperatorQualification, ShiftSchedule

**System** — Configuration, Sequence, ApplicationSetting, AuditLog, FileAttachment, IoTDevice, IoTTag, IntegrationMapping, ScheduledJob

---

## Screens

The package includes **56 screen files** providing core operational interfaces:

- Work order management and dispatch screens
- Shop floor operator control panel terminals
- Andon/request management submission and response screens
- Inventory management and transaction entry
- Work center and resource management dashboards
- Genealogy trace query and visualization screens
- System configuration and administration panels
- IoT device management and tag mapping screens
- Integration configuration and monitoring screens
- Application setup and deployment screens

---

## Access Control

The package establishes core platform roles:

| Role | Description |
|---|---|
| MES Administrator | Full system access including platform configuration and module management |
| Production Supervisor | Production order management, work center monitoring, Andon response |
| Shop Floor Operator | Production recording, labor capture, request submission |
| Inventory Analyst | Inventory management, cycle counts, adjustments |
| System Administrator | User management, access control, integration configuration |
| Integration Manager | EDI and ERP integration configuration and monitoring |

---

## Package Contents

```
mes-core/
├── manifest.json          # Package metadata (version 1.0.0)
├── definition.json        # Package structure and selection definitions
├── package-data.json      # All seed data (module registry, config tables)
├── data/                  # 34 seed data files
├── dataFlows/             # 32 data flow definitions
├── dataModels/            # 92 data model definitions
└── screens/               # 56 screen definitions
```

The **34 seed data records** establish the foundational platform configuration:
- Complete module group and module registry (18 groups, 41 modules)
- System configuration defaults and lookup tables
- Process type definitions and reason code templates
- Sequence number configuration for work orders, lots, and transactions

---

## Dependencies

| Dependency | Version | Required |
|---|---|---|
| Fuuz Industrial Operations Platform | `>= 2025.11.3` | Required |

> **Note:** This is the core MES foundation package. It provides the module registry and platform infrastructure used by all other Fuuz MES accelerators. For a complete production-ready MES deployment, see `application-mes-accelerator`. For warehouse-specific functionality, see `application-wms-accelerator`.

---

## Installation

1. Ensure your Fuuz platform instance is running version `>= 2025.11.3`
2. Navigate to **Platform > Packages** in your Fuuz tenant
3. Import the `mes-core` package (`.fuuz` file or directory import)
4. Run the module registry seeding flows to populate the module group and module tables
5. Configure roles and assign users per the Access Control section above
6. Apply system configuration defaults appropriate for your facility
7. Validate the deployment by confirming module navigation is accessible
8. Configure IoT device connectivity if using machine integration features
9. Set up NetSuite integration credentials if using the NetSuite connector module

For detailed setup and configuration documentation, see the [Fuuz Platform Documentation](https://help.fuuz.com).

## Service levels

No service level agreement applies to anything published here. It becomes a supported
deliverable only once it has been implemented by a Fuuz services professional or an
approved Fuuz partner.
