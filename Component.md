componentDiagram
    UI "用户界面" --> OrderService "订单处理服务"
    UI "用户界面" --> PaymentService "支付服务"
    UI "用户界面" --> InventoryService "库存管理服务"
    
    OrderService "订单处理服务" --> PaymentService "支付服务"
    OrderService "订单处理服务" --> InventoryService "库存管理服务"
    
    PaymentService "支付服务" --> Database "数据库"
    InventoryService "库存管理服务" --> Database "数据库"
    
    classDef default fill:#f9f,stroke:#333,stroke-width:2px;
