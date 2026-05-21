# Pellair Oils - Luxury B2B Shopify Theme

A sophisticated, exclusive Shopify theme designed specifically for Pellair Oils - a premium B2B fragrance oil business inspired by world-class perfume houses like Guerlain, Nasomatto, Orto Parisi, and more.

## 🌟 Features

### Business-to-Business (B2B) Focus
- **Business Registration System**: Comprehensive registration with business verification fields
- **Approval Workflow**: Customers tagged as "pending_approval" or "approved" for controlled access
- **Exclusive Access**: Checkout restricted until business approval is granted
- **B2B Pricing**: Special wholesale pricing for approved business partners

### Luxury Design
- **Dark & Elegant**: Sophisticated dark theme with gold (#c9a961) accents
- **Premium Typography**: Playfair Display for headings, Montserrat for body text
- **Responsive**: Fully mobile-optimized for all devices
- **Professional Imagery**: Designed to showcase luxury fragrance oil products

### Product Categorization
- **Brand Filtering**: Filter by luxury brands (Guerlain, Nasomatto, Orto Parisi, Xerjoff, etc.)
- **Accord Classification**: Organize by fragrance families (Floral, Woody, Oriental, Fresh, Citrus, Spicy, Oud, Leather, etc.)
- **Concentration Levels**: Filter by Parfum, EDP, EDT, EDC
- **Size Options**: Bulk ordering from 100g to 5kg+

### Product Features
- **Metafield Support**: 
  - Brand
  - Accord
  - Concentration
  - Top/Middle/Base Notes
  - Ingredients
  - Minimum Order Quantity
- **Image Gallery**: Multiple product images with thumbnail navigation
- **Tabbed Information**: Product details, fragrance notes, usage guidelines
- **Bulk Ordering**: Quantity controls optimized for B2B orders

### Customer Experience
- **Business Registration**: Detailed form with business name, type, tax ID, address
- **Account Dashboard**: Order history, account status, quick actions
- **Order Notes**: Special instructions for bulk orders
- **Password Recovery**: Complete authentication flow

## 📁 Theme Structure

```
pellair-oils-theme/
├── assets/
│   └── theme.css                    # Main stylesheet
├── config/
│   ├── settings_schema.json         # Theme customization options
│   └── settings_data.json           # Default settings
├── layout/
│   └── theme.liquid                 # Main layout template
├── locales/
│   └── en.default.json              # English translations
├── templates/
│   ├── 404.liquid                   # Error page
│   ├── cart.liquid                  # Shopping cart with B2B features
│   ├── collection.liquid            # Collection page with filters
│   ├── index.liquid                 # Homepage
│   ├── list-collections.liquid      # All collections
│   ├── page.liquid                  # Static pages
│   ├── product.liquid               # Product detail page
│   ├── search.liquid                # Search results
│   └── customers/
│       ├── account.liquid           # Customer dashboard
│       ├── activate_account.liquid  # Account activation
│       ├── login.liquid             # Login page
│       ├── register.liquid          # Business registration
│       └── reset_password.liquid    # Password reset
├── sections/                        # (Reserved for future sections)
└── snippets/                        # (Reserved for future snippets)
```

## 🚀 Installation

1. **Compress the theme folder** into a ZIP file
2. **Log into Shopify Admin**
3. Navigate to **Online Store > Themes**
4. Click **Upload theme**
5. Select the ZIP file
6. Click **Publish** when ready

## ⚙️ Configuration

### Theme Settings
Access via: **Online Store > Themes > Customize**

#### Colors
- Primary Color: #1a1a1a (Dark)
- Secondary Color: #c9a961 (Gold)
- Background: #0d0d0d (Very Dark)
- Text Color: #e8e8e8 (Light Gray)

#### Typography
- Headings: Playfair Display
- Body: Montserrat

#### B2B Settings
- Enable B2B Only Access
- Registration Required Message
- Approval Requirements Text

#### Brand Management
- Featured Brands List (comma-separated)
- Enable Brand Filtering
- Enable Accord Filtering

### Setting Up Products

#### Product Metafields
Add these metafields to products for full functionality:

1. **Brand** (custom.brand) - Text
2. **Accord** (custom.accord) - Text  
   Options: floral, woody, oriental, fresh, citrus, spicy, amber, aquatic, gourmand, leather, musk, oud
3. **Concentration** (custom.concentration) - Text
   Options: Parfum, EDP (Eau de Parfum), EDT (Eau de Toilette), EDC (Eau de Cologne)
4. **Top Notes** (custom.top_notes) - Multi-line text
5. **Middle Notes** (custom.middle_notes) - Multi-line text
6. **Base Notes** (custom.base_notes) - Multi-line text
7. **Ingredients** (custom.ingredients) - Multi-line text
8. **Minimum Order** (custom.minimum_order) - Number

### Customer Tags for B2B Workflow

#### Approval System
- **pending_approval**: Applied to new registrations awaiting verification
- **approved**: Applied after business verification - enables checkout

#### How to Approve Customers
1. Go to **Customers** in Shopify Admin
2. Open the customer record
3. In the **Tags** field, remove "pending_approval"
4. Add "approved"
5. **Send activation email** if needed

## 🎨 Customization

### Colors
Edit in **config/settings_schema.json** or through theme customizer:
- `color_primary`
- `color_secondary`
- `color_background`
- `color_text`
- `color_text_muted`

### Fonts
Change in theme settings or edit CSS variables in **layout/theme.liquid**

### Featured Brands
Update the brands list in theme settings:
`Guerlain,Nasomatto,Orto Parisi,Xerjoff,Initio,Baccarat Rouge,Creed,Tom Ford,Maison Francis Kurkdjian`

## 📦 B2B Features Guide

### Business Registration Process
1. Customer clicks "Register Your Business"
2. Fills detailed form with:
   - Personal info (name, email, password)
   - Business info (name, type, tax ID)
   - Contact details (phone, website, address)
   - Business description
3. Submission creates account with "pending_approval" tag
4. Admin reviews and approves
5. Customer receives activation email
6. Full access granted with B2B pricing

### Bulk Ordering
- Quantity selectors support large orders
- Minimum order quantities displayed
- Order notes for special requirements
- Cart optimized for B2B workflow

## 🛍️ Collections Setup

### Recommended Collections
1. **All Products** - Main catalog
2. **By Brand** - One collection per luxury brand
3. **By Accord** - Collections for each fragrance family
4. **New Arrivals** - Recently added products
5. **Best Sellers** - Popular items

## 📱 Responsive Design

Fully responsive breakpoints:
- Desktop: 1400px+
- Tablet: 768px - 1399px
- Mobile: < 768px

## 🔒 Security & Privacy

- Secure customer authentication
- Password recovery flow
- Business information protection
- HTTPS required for production

## 🎯 SEO Features

- Semantic HTML structure
- Proper heading hierarchy
- Meta descriptions support
- Canonical URLs
- Breadcrumb navigation
- Structured product data ready

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📞 Support & Maintenance

### Common Customizations
- Add more brands to filter list
- Modify color scheme
- Adjust typography
- Add custom pages
- Extend metafield options

### Performance Tips
- Optimize product images (WebP format recommended)
- Use Shopify CDN for assets
- Enable browser caching
- Minimize custom code

## 📄 License

This theme is proprietary and created exclusively for Pellair Oils.

## 🎨 Design Inspiration

This theme draws inspiration from luxury perfume houses:
- **Guerlain** - Classic elegance and sophistication
- **Nasomatto** - Bold and mysterious presentation
- **Orto Parisi** - Artisanal and exclusive feel
- **Xerjoff** - Opulent luxury aesthetic
- **Maison Francis Kurkdjian** - Modern refinement

## 🔄 Version History

**Version 1.0.0** (Initial Release)
- Complete B2B functionality
- Business registration and approval workflow
- Brand and accord filtering
- Product metafields support
- Responsive design
- Luxury dark theme
- Customer account management
- Bulk ordering features

---

**Created for Pellair Oils** - Exclusive Fragrance Oils for Discerning Businesses
