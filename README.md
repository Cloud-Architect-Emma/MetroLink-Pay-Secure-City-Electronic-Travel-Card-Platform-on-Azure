# Overview

This project presents a design-only, production-grade solution architecture for a cloud-native, contactless public transport payment system built on Microsoft Azure.

The system enables passengers to pay fares using an electronic travel card, with instant validation at the payment machine, while supporting offline operation, secure payment settlement, and operator-side enforcement.

#### Key Features

Contactless NFC-based fare validation

Offline-first transport operation

Account-based payment model

Secure external payment gateway integration

Real-time operator visibility

Privacy-by-design architecture

Multi-modal transport support

Event-driven, serverless Azure design

#### Architecture Flow
![Architecture-Flow](architecture/architecture-diagram-(7).gif).


#### Architecture Highlights

Azure IoT Hub for secure device ingestion

Azure Functions for fare calculation and payment orchestration

Azure Event Grid for event routing

Azure Cosmos DB for transaction state

Azure Blob Storage for audit logs

External PCI-compliant payment gateway (outside Azure boundary)

#### Payment Model

No card data stored in Azure

Payment authorization handled externally

Azure orchestrates and records payment outcomes only

Settlement occurs directly to transport operator accounts

**Author**

Designed by Emmanuela.
