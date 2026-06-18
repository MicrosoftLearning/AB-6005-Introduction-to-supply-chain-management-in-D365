## Exercise: Process a purchase order by using the Warehouse Management mobile app

### Objective

In this lab, you will become familiar with the operations of the Warehouse Management mobile app. You will also create a new purchase order and process the purchase receipt by using the Warehouse Management mobile app.

### Lab steps

### Create a purchase order

1.  On the **Finance and Operations** home page, in the upper right, verify you are working with the **USMF** company. If necessary, select the company, and from the drop-down list, select **USMF**.
1.  In the upper left, select the **Expand the navigation pane** hamburger menu.
1.  Select **Modules** \> **Procurement and sourcing** \> **Purchase orders** \> **All purchase orders**.
1.  On the **All purchase orders** page, in the upper menu, select **+New**.
1.  In the **Create purchase order** pane, select the **Vendor account** drop-down list, and then select **US-101**.
1.  Expand the **General** section if necessary.
1.  Under **STORAGE DIMENSIONS**, select the **Site** drop-down list, and review the list of sites. Select site number **2** from the lookup. From the **Warehouse** lookup, select **24** in the **Warehouse** field.
1.  Select **OK**.

    The order header has now been created. When you work with purchase order lines, only a summary of the header information is displayed. If you need to view the rest of the information, select **Header**.

1.  A new line should be automatically created under the **Purchase order line** FastTab. If not, select the **Add line** button to create a new purchase order line.
1. Select the **Item number** cell drop-down list, and then select **A0001**.

    A purchase order line will be created for item A0001.

    **Site** and **Warehouse** are typically populated with values from the order header, which are **2** and **24** respectively.

1. In the **Quantity** box, enter **10**.
1. Select the **Save** button in the action pane to save the purchase order.
1. To confirm the purchase order, select the **Purchase** menu in the action pane.
1. Under **Actions**, select the **Confirm** button to confirm the purchase order.
1. Note the purchase order number and close the **Purchase order** page.

### Add a new warehouse mobile user

1.  Navigate to **Warehouse management** \> **Setup** \> **Worker** page.
1.  Select the **New** button in the action pane.
1.  From the list of workers, select **Ted Howard** followed by the **Select** button.
1.  Select the **New** button in the **Users** FastTab.
1.  In the **User ID** field, enter **ted**.
1.  Enter **24** as the **Default warehouse.**
1.  Enter **Main** as the **Menu name**.
1.  Select the **Save** button in the action pane.

    The **Set password** dialog will appear.

1.  Enter **123** as the password.
1. Close the page.

### Warehouse Management mobile app emulator

1.  Open a new browser window with the finance and operations URL. Add **\&mi=action:WHSWorkExecute** in the URL. A new dialog box appears in the browser page, requesting **User ID** and **Password** to get into the Warehouse Management mobile emulator.
1.  Enter **ted** and **123** in the **User ID** and **Password** fields.
1.  Select the **Inbound** menu followed by the **Purchase Receive** menu.
1.  In the **PONum** field, enter the purchase order number that you noted earlier, and then select **OK**.
1.  When the **Item** field appears, enter **A0001** and select **OK**.

    In the **Unit** field, **pcs** will appear automatically.

1.  In the **Qty** field, enter **10** and select the **OK** button.

    A notification appears that says **Work is complete**.

1.  Select the **Cancel** button, which will take you back to the menu.

### Creation of work

1.  Navigate to **Warehouse management** \> **Work** \> **All work**.

    A new open work is created for the purchase order.

    When you enter the Work record, you will find two work lines. The first line will pick the items from **RECV** location, and the second line will put it in the **FL-001** location.

1.  Note the work number.

### Check on-hand quantity

1.  Navigate to **Product information management** \> **Products** \> **Released products**.
1.  Find the product **A0001** and navigate to the **Manage inventory** \> **View** \> **On-hand inventory** action pane.
1.  Select the **Dimensions** button in the action pane.
1.  In the **Dimensions display** dialog, select all the **Storage dimensions** (**Site**, **Warehouse**, **Location**, **License plate**, and **Inventory status**).
1.  Select the **Save setup** slider field followed by the **OK** button.

    A new entry appears in the **RECV** location of warehouse **24**, where a quantity of **10** is displayed in the **Physical inventory** column.

### Warehouse mobile app emulator

1.  Navigate back to the **Warehouse Management** mobile app emulator.
1.  Select the **Purchase Put-away** menu.
1.  In the **ID** field, enter the work number that you copied earlier, and then select **OK**.
1.  Select **OK** again.
1.  Select the **Done** button followed by the **OK** button.

    A notification appears that says Work completed.

| Note: Navigate back to the **Work** page. Notice that the work is closed. Navigate back to the **On-hand inventory** page. Notice that the quantity of 10 items is moved from the **RECV** location to the **FL-001** location.  |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

