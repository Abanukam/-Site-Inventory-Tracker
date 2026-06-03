{
  "system": {
    "name": "BuildStore 2026",
    "version": "1.0",
    "industry": "Construction",
    "type": "Cloud-Native Construction Store ERP",
    "platforms": [
      "Web",
      "Android",
      "iOS",
      "Tablet"
    ],
    "offline_mode": true,
    "real_time_sync": true,
    "multi_site_support": true,
    "ai_enabled": true
  },

  "users": {
    "roles": [
      {
        "role": "Super Admin",
        "permissions": ["full_access"]
      },
      {
        "role": "Store Manager",
        "permissions": [
          "inventory_management",
          "approvals",
          "reporting"
        ]
      },
      {
        "role": "Storekeeper",
        "permissions": [
          "receive_materials",
          "issue_materials",
          "stock_count"
        ]
      },
      {
        "role": "Procurement Officer",
        "permissions": [
          "purchase_orders",
          "supplier_management"
        ]
      },
      {
        "role": "Project Manager",
        "permissions": [
          "view_site_inventory",
          "approve_requests"
        ]
      },
      {
        "role": "Executive",
        "permissions": [
          "dashboard_access",
          "analytics"
        ]
      }
    ]
  },

  "modules": {

    "dashboard": {
      "widgets": [
        "total_inventory_value",
        "materials_received_today",
        "materials_issued_today",
        "low_stock_alerts",
        "pending_requests",
        "supplier_performance",
        "site_stock_comparison",
        "fuel_usage",
        "asset_status"
      ]
    },

    "inventory": {
      "features": [
        "real_time_stock_balance",
        "batch_tracking",
        "lot_tracking",
        "unit_conversion",
        "minimum_stock_levels",
        "maximum_stock_levels",
        "inventory_valuation",
        "material_category_management"
      ]
    },

    "goods_receiving": {
      "fields": [
        "grn_number",
        "supplier",
        "delivery_note",
        "purchase_order",
        "site",
        "received_by",
        "inspection_status",
        "attachments"
      ],
      "auto_generate_grn": true
    },

    "material_issue": {
      "fields": [
        "issue_number",
        "request_number",
        "site",
        "issued_to",
        "approved_by",
        "item",
        "quantity",
        "purpose"
      ],
      "auto_update_stock": true
    },

    "material_requests": {
      "workflow": [
        "submitted",
        "reviewed",
        "approved",
        "issued",
        "closed"
      ]
    },

    "stock_count": {
      "features": [
        "cycle_counting",
        "variance_detection",
        "investigation_tracking",
        "approval_workflow"
      ]
    },

    "suppliers": {
      "features": [
        "supplier_database",
        "supplier_scorecard",
        "delivery_performance",
        "quality_rating",
        "contract_management"
      ]
    },

    "assets": {
      "features": [
        "asset_registry",
        "equipment_tracking",
        "maintenance_schedule",
        "asset_lifecycle"
      ]
    },

    "fuel_management": {
      "features": [
        "fuel_issue_tracking",
        "equipment_consumption_analysis",
        "fuel_cost_reporting",
        "fuel_variance_monitoring"
      ]
    },

    "cost_control": {
      "features": [
        "material_cost_tracking",
        "budget_vs_actual",
        "project_cost_allocation",
        "wastage_monitoring"
      ]
    },

    "site_management": {
      "features": [
        "multi_site_inventory",
        "site_transfers",
        "site_comparison_dashboard",
        "site_performance_metrics"
      ]
    }
  },

  "automation": {

    "inventory_engine": {
      "formula": "opening + received - issued - damaged + transfers_in - transfers_out"
    },

    "alerts": {
      "low_stock": true,
      "overstock": true,
      "expired_materials": true,
      "delayed_deliveries": true,
      "unapproved_requests": true
    },

    "notifications": {
      "email": true,
      "sms": true,
      "push_notifications": true,
      "whatsapp": true
    }
  },

  "ai_features": {

    "forecasting": [
      "material_demand_prediction",
      "stock_reorder_prediction",
      "fuel_consumption_forecast"
    ],

    "assistant": [
      "natural_language_queries",
      "report_generation",
      "variance_explanations",
      "procurement_recommendations"
    ]
  },

  "security": {

    "authentication": [
      "email_login",
      "phone_login",
      "microsoft_login",
      "google_login"
    ],

    "authorization": [
      "role_based_access",
      "site_based_access"
    ],

    "audit_trail": true,
    "activity_logs": true,
    "data_encryption": true
  },

  "analytics": {

    "reports": [
      "daily_store_report",
      "weekly_store_report",
      "monthly_inventory_report",
      "material_consumption_report",
      "supplier_performance_report",
      "fuel_usage_report",
      "project_cost_report",
      "stock_variance_report"
    ],

    "visualizations": [
      "charts",
      "heatmaps",
      "trend_analysis",
      "executive_scorecards"
    ]
  },

  "mobile_app": {

    "features": [
      "barcode_scanning",
      "qr_code_scanning",
      "photo_capture",
      "offline_transactions",
      "voice_data_entry",
      "gps_site_verification"
    ]
  },

  "database": {

    "entities": [
      "users",
      "sites",
      "materials",
      "suppliers",
      "purchase_orders",
      "goods_receipts",
      "material_requests",
      "issues",
      "stock_balances",
      "stock_counts",
      "assets",
      "fuel_records",
      "audit_logs"
    ]
  },

  "technology_stack": {

    "frontend": [
      "Next.js",
      "React",
      "Tailwind CSS"
    ],

    "mobile": [
      "Flutter"
    ],

    "backend": [
      "NestJS"
    ],

    "database": [
      "PostgreSQL"
    ],

    "cache": [
      "Redis"
    ],

    "storage": [
      "AWS S3"
    ],

    "ai": [
      "OpenAI",
      "Predictive Analytics Engine"
    ]
  }
}
