```mermaid
graph TD
    A[Customer Order Request] --> B{Order Management Service}
    B --> C{Customer Profile Service}
    B --> D{Measurement Service}
    B --> E{Inventory Service}
    B --> F{Payment Gateway}
    B --> G{Production Service}
    G --> H{Tailor Assignment}
    G --> I{Work-in-Progress (WIP) Tracking}
    G --> J{Quality Control}
    J --> K{Packaging & Dispatch}
    K --> L[Shipping Carrier API]
    L --> M[Customer Notification (WhatsApp/Email)]
    F --> N[Payment Confirmation]
    N --> P[Accounting System Update]
    P --> Q[Reporting Dashboard]

    subgraph Order Management Flow
        A(Customer initiates order)
        B{OMS processes order}
        C[Fetch customer data]
        D[Retrieve measurements]
        E[Check fabric/material availability]
        F[Process payment]
        G[Initiate production order]
        H[Assign to tailor]
        I[Track production stages]
        J[Perform QC checks]
        K[Prepare for dispatch]
        L[Generate shipping label & tracking]
        M[Notify customer]
        N[Confirm payment]
        P[Update accounting ledger]
        Q[Update dashboards]
    end
