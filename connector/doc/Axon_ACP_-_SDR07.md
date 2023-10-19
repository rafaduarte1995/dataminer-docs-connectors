---
uid: Connector_help_Axon_ACP_-_SDR07
---

# Axon ACP - SDR07

The SDR07 is a triple-channel reclocking distribution amplifier compatible with ASI/DVB.

The **Axon ACP - SDR07** connector can be used to display and configure information of the related device.

## About

This connector is automatically generated by the connector **Axon ACP**.

There are also different possibilities available for **alarm monitoring** and **trending**.

### Version Info

| **Range** | **Description**                    | **DCF Integration** | **Cassandra Compliant** |
|-----------|------------------------------------|---------------------|-------------------------|
| 1.0.1.x   | Extended parameters.               | No                  | Yes                     |
| 1.0.2.x   | Change in export rules.            | Yes                 | Yes                     |
| 1.0.3.x   | Change in discrete display values. | Yes                 | Yes                     |

### Product Info

| Range     | Supported Firmware     |
|-----------|------------------------|
| 1.0.1.x   | 0100, 0200, 0300       |
| 1.0.2.x   | 0100, 0200, 0300       |
| 1.0.3.x   | 0100, 0200, 0300       |

## Configuration

The element is automatically created by the parent element using the **Axon ACP** connector.

## Usage

### General

This page displays general information about the card: **Card Name**, **Card Description**, **SW Revision**, **HW Revision**, etc.

### Amplifier

On this page, you can find the status and settings related to the amplifier.

### Alarm Priority

This page displays the event messages of the card, i.e. special messages generated asynchronously on the card.

## DataMiner Connectivity Framework

The Axon ACP connector supports the usage of DCF and can only be used on a DMA with 8.5.4 as the minimum version.

DCF can also be implemented through the DataMiner DCF user interface and throught DataMiner third-party connectors (for instance a manager).

Connectivity for this connector is managed by the parent connector Axon ACP.

### Interfaces

#### Physical Interfaces

- **SDI Input A**: A single fixed interface of type **input**.
- **SDI Input B**: A single fixed interface of type **input**.
- **SDI Input C**: A single fixed interface of type **input**.
- **SDI Output A1**: A single fixed interface of type **output**.
- **SDI Output A2**: A single fixed interface of type **output**.
- **SDI Output B1**: A single fixed interface of type **output**.
- **SDI Output B2**: A single fixed interface of type **output**.
- **SDI Output C1**: A single fixed interface of type **output**.
- **SDI Output C2**: A single fixed interface of type **output**.

#### Virtual Interfaces

- **Reclocker A**: A single fixed interface of type **inout**.
- **Reclocker B**: A single fixed interface of type **inout**.
- **Reclocker C**: A single fixed interface of type **inout**.

### Connections

#### Internal Connections

When a DVE child element is created, the following connections are established:

- Between **SDI Input A** and **Reclocker A**
- Between **Reclocker A** and **SDI Output A1**
- Between **Reclocker A** and **SDI Output A2**
- Between **SDI Input B** and **Reclocker B**
- Between **Reclocker B** and **SDI Output B1**
- Between **Reclocker B** and **SDI Output B2**
- Between **SDI Input C** and **Reclocker C**
- Between **Reclocker C** and **SDI Output C1**
- Between **Reclocker C** and **SDI Output C2**