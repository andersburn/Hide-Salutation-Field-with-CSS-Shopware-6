# Hide Salutation Field with CSS

This simple snippet hides the salutation (Mr./Ms.) field across various Shopware forms using CSS only.  
It’s a non-destructive solution — no core modifications, no plugin conflicts.

## How to Use
Add the following CSS to your theme or custom stylesheet:

```css
.row.g-2:has(select#personalSalutation),
.row.g-2:has(select#shipping-edit-addresspersonalSalutation),
.row.g-2:has(select#shipping-new-addresspersonalSalutation),
.row.g-2:has(select#billing-new-addresspersonalSalutation),
.row.g-2:has(select#billing-edit-addresspersonalSalutation),
.row.g-2:has(select#shippingAddresspersonalSalutation),
.form-group.col-md-4:has(select#form-Salutation)
{
    display: none !important;
}

```
Notes
- This snippet is designed for the default Shopware theme.
- Custom themes may require small adjustments.
- Use !important if the default CSS still displays the field.
