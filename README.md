# 🎯 Custom File Upload Section (Product Add-to-Cart)
## Overview

The Custom File Upload Section allows customers to upload one or multiple files directly on the product page before adding the product to the cart.
Uploaded files are securely attached to the cart item as line item properties, making them visible in the Shopify admin and order details.

This section is ideal for stores that require customer-provided files during checkout, such as:

  - Printing & signage stores (artwork, PDFs, designs)

  -  Custom apparel (logos, images)

  - Engraving or personalization services

  - Any made-to-order product requiring customer assets

The section is fully customizable through the Shopify Theme Editor and works with both standard add-to-cart and AJAX cart / drawer systems (including Minimog-style themes).

# ✅ How to Install

Follow these steps to install and use the Custom File Upload section in your Shopify theme:

1. Open Your Shopify Theme Code Editor

- From your Shopify admin, go to: Online Store → Themes

- Find your active theme, then click ⋯ (More) → Edit code.

2. Create a New Section

- In the Sections folder, click Add a new section

- Name the file (e.g. custom-file-upload.liquid)

- Paste the entire section code into the new file

Click Save

# ✅ How to Use
## 1. Add the Section to a Product Page

- Open Online Store → Themes → Customize

- Navigate to a Product page

- Click Add section

- Select Custom File Upload

## ⚠️ Important:
This section must be used on a product page that contains an Add to Cart button.

## 2. Configure Section Settings

- All options are available inside the Theme Editor:

- General Settings

- Title – Section heading (e.g. “Upload Artwork”)

- Label (Property Name): Name shown in order details (e.g. “Design”)

- Max Files: Number of files a customer can upload

- Accepted File Types: Control allowed formats
Example: image/*,.pdf,.ai,.psd

Upload Area Text

- Dropzone Text: Instruction text inside upload area

- Button Text: Text for the “Select File” button

## 3. Styling & Design Controls

- Background Color

- Text Color

- Accent Color (icons)

- Border Color

- Dropzone Background

- Button Background & Text Color

- Border Radius (container, dropzone, button)

- All styling updates apply instantly without editing code.

# 🛒 How It Works (Technical Flow)

Customers select or upload files before clicking Add to Cart

Files are attached to the product as line item properties

The product form is automatically converted to multipart/form-data

On submission:

Files are sent using Shopify’s /cart/add.js

Cart drawer or cart page updates automatically

Uploaded files appear in:

Shopify Admin → Orders

Order details

Cart line item properties

Image files show live previews; non-image files display a document icon.

## 💡 Best Use Cases

Printing stores requiring customer artwork

Custom merchandise and branding orders

Personalized gifts

Manufacturing workflows requiring design files

# ✅ Compatibility

Works with standard Shopify themes

Supports AJAX add to cart

Compatible with cart drawers

Includes fallback to normal form submit if AJAX fails

Supports dynamic product forms and theme reloads

# 🧩 Tips

- Set Max Files according to your workflow to avoid unnecessary uploads

- Restrict file types to prevent unsupported formats

- Use clear instructional text to reduce customer errors

- For large files, advise customers about size limits (Shopify standard limits apply)

# ⚠️ Troubleshooting

- Files not attaching to the order?
→ Ensure the section is placed on a product page with a valid Add to Cart form.

- Cart drawer not updating?
→ Your theme must listen for cart:updated or cart:refresh events (already handled for most modern themes).

- Images not previewing?
→ Only image MIME types (image/*) generate previews. Other formats will show a document icon.

- Button not working?
→ Ensure no conflicting custom scripts override the product form submit behavior.

# ✅ Summary

The Custom File Upload Section provides a clean, professional, and reliable way to collect customer files during the add-to-cart process, without third-party apps.

It improves order accuracy, reduces back-and-forth communication, and is fully customizable from the Shopify Theme Editor.

Ideal for any store that depends on customer-submitted files to fulfill orders.
