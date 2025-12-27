# How to Use - Mobile Repair System

## Quick Start Guide

### For Owners

#### 1. Initial Setup
```
Login → Dashboard
├─ Create your first shop
├─ Add device categories
├─ Create repair services
└─ Add parts to inventory
```

#### 2. Add Managers
```
Dashboard → Managers → Create Manager
├─ Enter manager details
├─ Assign to shop
└─ Manager receives login credentials
```

#### 3. Stock Setup
```
Dashboard → Inventory → Stock
├─ Select category (iPhone 13, Samsung S21, etc.)
├─ Use bulk grid to add multiple parts
└─ Save - stock is now available
```

#### 4. Monitor Business
```
Dashboard → Reports
├─ Repair Report - See all repairs
├─ Purchase Report - Track spending
└─ Parts Used - Analyze inventory usage
```

---

### For Managers

#### 1. Daily Workflow
```
Login → Dashboard
├─ Check active repairs
├─ View today's bookings
└─ Monitor pending payments
```

#### 2. Creating a Repair Booking
```
Repair Bookings → Add Repair
├─ Select customer (or create new)
├─ Choose category/subcategory
├─ Select repair service
├─ Set device attributes (color, storage, etc.)
├─ Enter price and advance payment
└─ Save booking
```

#### 3. Managing Repairs
```
Update Status:
├─ Click status badge → Change to In Progress/Fixed/etc.

Update Payment:
├─ Click payment badge → Mark as Paid
├─ Select payment type (Cash/Card)

Add Parts Used:
├─ Click "Add parts" in Parts column
├─ Select parts from list
├─ Stock automatically decreases
└─ Save
```

#### 4. Using Kanban Board
```
Kanban Board
├─ See all repairs as cards
├─ Drag card to new status column
├─ Status updates automatically
└─ Quick visual overview
```

---

## Common Tasks

### Create a New Shop (Owner)
1. Dashboard → Shops → Create Shop
2. Enter shop name, address, contact
3. Save
4. Shop is now available for manager assignment

### Add Stock (Owner/Manager)
1. Inventory → Stock → Add Stock
2. Select category (e.g., iPhone 13)
3. Click "Use Grid Entry" for multiple parts
4. Enter quantities for each part
5. Save - stock is updated

### Process a Repair (Manager)
1. **Create Booking**
   - Repair Bookings → Add Repair
   - Fill in customer and device details
   - Set price

2. **Update as Work Progresses**
   - Change status: Booked → In Progress → Fixed
   - Add parts used (stock decreases automatically)
   
3. **Mark as Paid**
   - Click payment badge
   - Select Paid + payment type

4. **Customer Collects**
   - Change status to Customer Collected
   - Collection date auto-set

### Generate Reports (Owner/Manager)
1. Reports → Select report type
2. Apply filters:
   - Date range
   - Shop (owner only)
   - Category/Status
3. View stats and listings
4. Click for detailed information

### Customize Email Template (Manager)
1. Email Templates → Click template card
2. Edit subject and body
3. Insert variables by clicking them
4. Save - shop-specific template created
5. Reset button returns to owner's template

---

## Understanding the System

### Stock Management
```
When you ADD parts to booking:
→ Stock DECREASES by quantity used

When you REMOVE parts from booking:
→ Stock INCREASES (restored)

If stock doesn't exist:
→ Creates negative stock (-1, -2, etc.)
→ When you add stock later, it balances out
```

### Category Structure
```
Parent: iPhone
  ├─ iPhone 13 (stock tracked separately)
  ├─ iPhone 14 (stock tracked separately)
  └─ iPhone 15 (stock tracked separately)

Parent: Samsung
  ├─ Galaxy S21 (stock tracked separately)
  └─ Galaxy S22 (stock tracked separately)
```

### Permissions
```
Owner Can:
✅ Manage all shops
✅ Create categories, parts, services
✅ View all data
✅ Configure global settings

Manager Can:
✅ Manage repairs for their shop only
✅ View categories, parts, services (read-only)
✅ Add stock for their shop
✅ View reports for their shop only
✅ Customize email templates
```

### Currency System
```
Priority:
1. Shop Currency (if set by manager)
2. Owner Currency (if shop not set)
3. USD (default)

All prices display in active currency
Changes apply immediately
```

### Email System
```
SMTP Priority:
1. Shop SMTP (if configured)
2. Owner SMTP (if shop not set)
3. Default .env SMTP

Template Priority:
1. Shop-customized template
2. Owner template
3. System default
```

---

## Tips & Best Practices

### For Owners

**Setup Order:**
1. Categories first (device types)
2. Services (repair types)
3. Parts (inventory items)
4. Shops
5. Managers
6. Stock

**Regular Tasks:**
- Check reports weekly
- Monitor stock levels
- Review shop performance
- Update pricing as needed

### For Managers

**Daily Workflow:**
1. Check dashboard for active repairs
2. Update repair statuses
3. Add parts as used
4. Mark payments when received
5. Update customer collected status

**Inventory:**
- Add parts immediately when used
- Request stock from owner when low
- Use bulk grid for efficiency

**Customer Service:**
- Update status promptly
- Send email confirmations
- Keep customers informed

---

## Keyboard Shortcuts

### Navigation
- `/` - Focus search (if available)
- `Esc` - Close modal/drawer

### Forms
- `Enter` - Submit form
- `Tab` - Next field
- `Shift + Tab` - Previous field

---

## Troubleshooting

### "Stock not available"
- Check if part exists for that category
- Negative stock is allowed (can still use)
- Contact owner to add stock

### "Cannot see shop in filter"
- Managers: You only see your assigned shop
- Owners: Check if shop is active

### "Email not sending"
- Check SMTP settings
- Verify email template exists
- Check server mail logs

### "Cannot change status"
- Ensure repair exists
- Check permissions
- Refresh page and try again

---

## Getting Help

### In-App Support
- Settings → Help
- Hover tooltips on forms
- Error messages guide you

### Contact
- Owner: Contact system administrator
- Manager: Contact your shop owner
