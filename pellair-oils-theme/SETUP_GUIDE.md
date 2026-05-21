# Pellair Oils Theme - Quick Setup Guide

## 🚀 Quick Start (5 Minutes)

### Step 1: Install Theme
1. Compress the `pellair-oils-theme` folder into a ZIP file
2. Log into your Shopify Admin
3. Go to **Online Store > Themes**
4. Click **Upload theme** button
5. Select your ZIP file and upload
6. Once uploaded, click **Publish**

### Step 2: Configure Metafields (Required)
Product metafields are essential for brand and accord filtering.

1. Go to **Settings > Custom Data > Products**
2. Click **Add definition**
3. Create these metafields:

| Name | Namespace & Key | Type | Description |
|------|----------------|------|-------------|
| Brand | custom.brand | Single line text | e.g., "Guerlain" |
| Accord | custom.accord | Single line text | e.g., "floral" |
| Concentration | custom.concentration | Single line text | e.g., "EDP" |
| Top Notes | custom.top_notes | Multi-line text | First impression notes |
| Middle Notes | custom.middle_notes | Multi-line text | Heart notes |
| Base Notes | custom.base_notes | Multi-line text | Lasting notes |
| Ingredients | custom.ingredients | Multi-line text | Full ingredient list |
| Minimum Order | custom.minimum_order | Integer | Min units required |

### Step 3: Add Products
1. Go to **Products > Add product**
2. Add product details (title, description, price, images)
3. In the **Metafields** section, add:
   - Brand: One of your luxury brands
   - Accord: One of: floral, woody, oriental, fresh, citrus, spicy, oud, leather
   - Concentration: Parfum, EDP, EDT, or EDC
   - Notes: Top, Middle, Base notes
4. Click **Save**

### Step 4: Set Up Customer Tags
For B2B approval workflow:

1. When a customer registers, they automatically get tagged
2. To approve a customer:
   - Go to **Customers**
   - Click on the customer
   - In **Tags**, add: `approved`
   - Remove: `pending_approval` (if present)
   - Save

### Step 5: Create Collections
1. **All Products Collection**
   - Go to **Products > Collections > Create collection**
   - Title: "All Products"
   - Automated: All products
   
2. **Brand Collections** (Optional but recommended)
   - Create one collection per brand
   - Use metafield filtering: custom.brand equals "Guerlain"
   
3. **Accord Collections** (Optional but recommended)
   - Create collections for each accord
   - Use metafield filtering: custom.accord equals "floral"

## 🎨 Theme Customization

### Access Theme Settings
**Online Store > Themes > Customize**

### Key Settings to Configure

#### 1. Colors (Optional - defaults are set)
- Primary Color: Dark tone
- Secondary Color: Gold accent
- Background: Very dark
- Text colors

#### 2. Homepage
- Hero Title: "Pellair Oils" (or your business name)
- Hero Subtitle: Your tagline
- Hero Image: Upload a luxury background image (optional)

#### 3. B2B Settings
- ✅ Enable B2B Only Access (recommended)
- Registration Message: Customize the message shown to visitors
- Approval Requirements: Explain what documents/info you need

#### 4. Brand List
Update the featured brands list (comma-separated):
```
Guerlain,Nasomatto,Orto Parisi,Xerjoff,Initio,Baccarat Rouge,Creed,Tom Ford,Maison Francis Kurkdjian
```

## 📧 Customer Flow

### New Customer Registration
1. Customer visits your site
2. Clicks "Register Your Business"
3. Fills out detailed form:
   - Personal information
   - Business details
   - Tax ID / Business registration number
4. Submits form
5. Sees "pending approval" message

### Admin Approval Process
1. Receive notification of new registration
2. Review customer details in Shopify Admin
3. Verify business legitimacy (check tax ID, website, etc.)
4. Add `approved` tag to customer
5. Customer can now checkout with B2B pricing

## 🛠️ Advanced Configuration

### Navigation Menu
**Online Store > Navigation > Main menu**

Recommended structure:
```
- Home (/)
- Collections (/collections/all)
  - All Products (/collections/all)
  - Shop by Brand (/collections/brands)
  - Shop by Accord (/collections/accords)
- About (/pages/about)
- Contact (/pages/contact)
```

### Create Essential Pages
**Online Store > Pages > Add page**

Recommended pages:
1. **About Us** - Company story
2. **Contact** - Contact form and details
3. **B2B Registration** - Explain registration process
4. **Quality Guarantee** - Product quality information
5. **Shipping Information** - Delivery details
6. **Terms & Conditions** - Legal terms
7. **Privacy Policy** - Privacy information
8. **FAQ** - Common questions

### Email Notifications
**Settings > Notifications**

Customize these templates to match your branding:
- Customer account welcome
- Customer account activation
- Order confirmation
- Order shipped

## 🎯 Product Setup Best Practices

### Image Guidelines
- **Main Image**: 3:4 ratio (e.g., 1200x1600px)
- **Format**: JPG or PNG, optimized for web
- **Style**: Match the luxury aesthetic (dark background, professional lighting)
- Show product bottle/container clearly

### Product Descriptions
Write detailed descriptions including:
- Inspiration (which luxury perfume it's inspired by)
- Scent profile
- Use cases (candles, soaps, perfumes)
- Concentration level
- Size/volume information

### Pricing Strategy
- Set regular prices for retail
- Use customer tags for B2B pricing
- Consider quantity discounts via Shopify apps

## 🔍 SEO Setup

### Product SEO
For each product, optimize:
- **Title**: Include brand and scent name
- **Description**: Include keywords naturally
- **URL Handle**: Clean, readable URLs
- **Meta Description**: Compelling 155-character summary

### Homepage SEO
**Online Store > Preferences**
- Homepage title
- Homepage meta description
- Social sharing image

## 🛒 Checkout Configuration

### Checkout Settings
**Settings > Checkout**

Recommended:
- ✅ Require account to checkout (for B2B control)
- ✅ Email marketing opt-in
- Add any required business fields
- Configure shipping zones
- Set up payment providers

## 📱 Test Your Theme

### Testing Checklist
- [ ] Register a test business account
- [ ] Approve the test account (add "approved" tag)
- [ ] Add products to cart
- [ ] Complete a test order
- [ ] Check mobile responsiveness
- [ ] Test all navigation links
- [ ] Verify filters work (brand, accord)
- [ ] Test search functionality
- [ ] Check customer account dashboard

### Mobile Testing
Test on:
- iPhone (Safari)
- Android (Chrome)
- iPad/Tablet

## 🎓 Product Metafield Examples

### Example Product: "Guerlain Shalimar EDT"
```
Brand: Guerlain
Accord: oriental
Concentration: EDT
Top Notes: Bergamot, Lemon, Mandarin
Middle Notes: Iris, Jasmine, Rose
Base Notes: Vanilla, Tonka Bean, Incense
Minimum Order: 100
```

### Example Product: "Nasomatto Black Afgano"
```
Brand: Nasomatto
Accord: oud
Concentration: Parfum
Top Notes: Cannabis, Green Notes
Middle Notes: Coffee, Tobacco
Base Notes: Oud, Resins, Woods
Minimum Order: 50
```

## 🆘 Troubleshooting

### Filters Not Working?
- Ensure products have metafields set
- Check spelling of metafield values (case-sensitive)
- Clear browser cache

### Customer Can't Checkout?
- Verify customer has "approved" tag
- Check B2B settings are enabled
- Ensure customer is logged in

### Images Not Showing?
- Check image file size (max 20MB)
- Verify image format (JPG, PNG)
- Re-upload images if needed

### Styling Issues?
- Clear browser cache
- Check theme is published
- Verify CSS file loaded correctly

## 📞 Need Help?

### Resources
- Shopify Help Center: help.shopify.com
- Shopify Community: community.shopify.com
- Theme Documentation: See README.md

### Before Launching
- [ ] Test with real business registration
- [ ] Set up payment gateway
- [ ] Configure shipping rates
- [ ] Set up tax calculations
- [ ] Review legal pages (terms, privacy)
- [ ] Test checkout process end-to-end
- [ ] Verify email notifications
- [ ] Check mobile experience
- [ ] Set up analytics (Google Analytics)
- [ ] Add domain name

## 🚀 Launch Checklist

- [ ] Theme published and tested
- [ ] Products added with proper metafields
- [ ] Collections created
- [ ] Navigation menu configured
- [ ] Essential pages created
- [ ] Customer approval workflow tested
- [ ] Payment gateway connected
- [ ] Shipping zones configured
- [ ] Email notifications customized
- [ ] Mobile-responsive verified
- [ ] SEO optimized
- [ ] Analytics set up
- [ ] Domain connected
- [ ] SSL certificate active
- [ ] Legal pages complete

---

**Ready to go live!** 🎉

Your luxury B2B fragrance oil store is ready to serve discerning business clients.
