# TechCorp Services

This documentation covers the microservices at TechCorp.

## Service Catalog

### Product API
- **System**: Customer Portal
- **Technology**: Node.js, Express
- **Purpose**: Manage product catalog and inventory
- **Endpoints**:
  - `GET /api/products` - List all products
  - `GET /api/products/:id` - Get product details
  - `POST /api/products` - Create new product
  - `PUT /api/products/:id` - Update product
  - `DELETE /api/products/:id` - Remove product

### Payment API
- **System**: Payment Processing
- **Technology**: Java, Spring Boot
- **Purpose**: Process payments securely
- **Compliance**: PCI DSS Level 1
- **Endpoints**:
  - `POST /api/payments` - Process payment
  - `GET /api/payments/:id` - Get payment status
  - `POST /api/refunds` - Issue refund

### Catalog Backend
- **System**: Developer Portal
- **Technology**: Backstage, TypeScript
- **Purpose**: Backend service for Backstage catalog
- **Features**: Entity storage, catalog API, search indexing

## Architecture Patterns

All services follow these patterns:
- **API Gateway**: Kong for external traffic
- **Service Mesh**: Istio for internal communication
- **Observability**: Prometheus metrics, Jaeger tracing
- **CI/CD**: GitHub Actions with automated deployments
