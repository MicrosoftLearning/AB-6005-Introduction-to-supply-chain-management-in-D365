## Exercise: Create a purchase order

### Objective

In this lab, you will become familiar with the user interface and the different fields available in the purchase order form. You will also learn how to create and confirm a new purchase order.

### Lab steps

1.  On the **Finance and Operations** home page, in the upper right, verify you are working with the **USMF** company. If necessary, select the company, and from the drop-down list, select **USMF**.
1.  In the upper left, select the **Expand the navigation pane** hamburger menu.
1.  Select **Modules** \> **Procurement and sourcing** \> **Purchase orders** \> **All purchase orders**.
1.  On the **All purchase orders** page, in the upper menu, select **+New**.
1.  In the **Create purchase order** pane, select the **Vendor account** drop-down list, and then select **US-101**.

    **Note:** When you select a vendor, details from the vendor record, such as address, invoice account, delivery terms, and delivery mode, will be copied as default values into the order header. You can change these values at any time.

1.  Expand the **General** section if necessary.
1.  Under **STORAGE DIMENSIONS**, select the **Site** drop-down list, and review the list of sites. Select site number **1** from the lookup. From the **Warehouse** lookup, select **13** in the **Warehouse** field.

    The **Site** field, together with the **Warehouse** field, specify where the procured goods or services must be delivered. The default delivery address is the site. You can populate both fields with values set up for the selected vendor, or you can specify them manually.

1.  Under **DATES**, in the **Delivery date** field, you can specify when procured goods and services need to be delivered.

    You can specify a single delivery date for the order or provide unique delivery dates for the individual order lines. If the specified delivery date cannot be met for specific products or services because they have longer lead times, then those lines will be updated automatically with a later delivery date based on defined purchase lead time.

1.  Expand the **Administration** section. You can use the **Orderer** box to specify who is placing the order.

    This may be convenient to share with the vendor in case they need to contact that person. The value may be assigned automatically if the current user account is associated with a name on the **Users** page.

1. Select **OK**.

    The order header has now been created. When you work with purchase order lines, only a summary of the header information is displayed. If you need to view the rest of the information, select **Header**.

:::image type="content" source="./media/create-a-purchase-order/purchase-order-header-summary.png" alt-text="Purchase order page showing the order header summary area with Header available to view full header information.":::

1.  Under **Purchase order lines**, on the menu, select **Purchase order line**.

:::image type="content" source="./media/create-a-purchase-order/purchase-order-lines.png" alt-text="Purchase order lines section showing where to add and edit line item details.":::

1.  Under **DISPLAY**, select **Dimensions**.

    Products can be in variants that are differentiated by dimensions, such as color, size, or style. You can also set up products to use storage dimensions, such as site and warehouse or use optional tracking dimensions, such as batch and serial numbers. To improve order entry efficiency, you can add commonly used dimension fields directly to the order grid.

1.  In the **Dimensions display** panel, under **PRODUCT DIMENSIONS**, select the **Color** checkbox.

    **Optional:** If you select the **Save setup** switch, the dimensions you chose will also be displayed on the order line grid the next time you open the **Purchase order** page.

1.  Select **OK**.
1.  Select the **Item number** cell drop-down list, and then select **T0004**.

    A purchase order line will be created for item T0004.

1.  Select the **Color** drop-down list, review the available options, and then select **Black**.
1.  **Site** and **Warehouse** are typically populated with values from the order header, which are **1** and **13** respectively. You can override the fields if some lines need to be delivered to different locations.
1.  In the **Quantity** box, enter **10**.

    The **Quantity** is automatically populated with the minimum order quantity for the product if this is set up, or with the value of **1**.

1.  Additional fields include:
    -   **Unit**: Indicates the unit of measure for the ordered quantity. Normally, the unit is automatically provided from the purchasing unit on the product master data.
    -   **Unit price**: Contains a value from either a purchase agreement or a trade agreement. You can change the unit price on individual order lines; for example, if a unique price is negotiated with the vendor.
    -   **Discount**: Represents a discount amount per unit. This discount reduces the unit price by the discount. The discount is commonly supplied automatically from purchase agreements or trade agreements, but you can override the discount on individual lines if unique discounts were negotiated with the vendor.
    -   **Discount percentage**: When entered, this reduces the net amount for the line accordingly. The discount percentage is often supplied automatically from purchase agreements or trade agreements, but you can override this on individual lines if a unique discount percentage has been negotiated with the vendor.
    -   **Net amount**: Calculated from other fields on the line, including quantity, unit price, discount, and discount percent. If you change the net amount, the Unit Price, Discount, and Discount percent fields will be blank. When you post the purchase line without unit price, the amount posted will be proportionately divided based on the quantity purchased while calculating the cost.
1.  Under the purchase order lines, at the bottom of the page, select **Line details**.
1. Select the **Delivery** tab.

    You can assign a unique delivery date to each order line. The date is inherited from the field on the purchase order header, but you can change this.

1. Select the **Save** button in the action pane to save the purchase order.
1. To confirm the purchase order, select the **Purchase** menu in the action pane.
1. Under **Actions**, select the **Confirm** button to confirm the purchase order.
1. Close the **Purchase order** page.
1. On the **All purchase orders** page, use the **Filter** feature and find your new purchase order.
1. When complete, close the **All purchase orders** page and return to the home page.

