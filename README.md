```mermaid
graph TD
    A[Customer Order Request] --> B[Order Management Service]
    B --> C[Customer Profile Service]
    B --> D[Measurement Service]
    B --> E[Inventory Service]
    B --> F[Payment Gateway]
    B --> G[Production Service]
    G --> H[Tailor Assignment]
    G --> I[Work-in-Progress (WIP) Tracking]
    G --> J[Quality Control]
    J --> K[Packaging & Dispatch]
    K --> L[Shipping Carrier API]
    L --> M[Customer Notification (WhatsApp/Email)]
    F --> N[Payment Confirmation]
    N --> P[Accounting System Update]
    P --> Q[Reporting Dashboard]

    subgraph "Order Management Flow"
        A
        B
        C
        D
        E
        F
        G
        H
        I
        J
        K
        L
        M
        N
        P
        Q
    end
