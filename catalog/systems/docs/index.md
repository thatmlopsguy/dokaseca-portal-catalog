# TechCorp Systems

This documentation covers the systems architecture at TechCorp.

## System Overview

### Customer Portal
- **Domain**: E-commerce
- **Type**: Frontend web application
- **Purpose**: Customer-facing shopping interface
- **Tech Stack**: React, TypeScript
- **Components**: Product API integration, shopping cart, checkout flow

### Payment Processing
- **Domain**: Payments
- **Type**: Backend system
- **Purpose**: Process financial transactions securely
- **Tech Stack**: Java, Spring Boot
- **Compliance**: PCI DSS Level 1
- **Components**: Payment API, transaction processor, fraud detection

### Developer Portal
- **Domain**: Platform
- **Type**: Internal platform
- **Purpose**: Developer experience and productivity tools
- **Tech Stack**: Backstage, TypeScript, PostgreSQL
- **Features**: Service catalog, TechDocs, scaffolding templates

## Integration Patterns

Systems communicate via REST APIs and event-driven patterns using message queues for asynchronous processing.
