### Objective

In Contoso Entertainment System USA (USMF), you plan to purchase a new configuration of a cabinet from a vendor. You need to create an item to represent the new configuration. In this lab, you will learn how to create a new item and item configurations.

### Lab steps

In Contoso Entertainment System USA (USMF), you plan to purchase a new configuration of a cabinet from a vendor. You need to create an item to represent the new configuration.

1. On the Finance and Operations home page, in the upper-right corner, verify that you are working in **USMF**. If needed, select **USMF** from the company drop-down list.
1. In the upper-left corner, select **Expand the navigation pane**.
1. In the navigation pane, select **Modules** > **Product information management**. Then, on the **Products** menu, select **Products**.
1. On the **Products** page, select **+ New**.
1. On the **New product** page, verify that **Product type** is set to **Item**.
1. Verify that **Product subtype** is set to **Product**.
1. Under **Identification**, in **Product number**, enter **GTL007**.
1. In **Product name**, enter **Cabinet 2**.

:::image type="content" source="./media/create-a-product/new-product-form.png" alt-text="New product page with Product type set to Item, Product subtype set to Product, Product number GTL007, and Product name Cabinet 2.":::

1. Select **OK**.
1. In the Action Pane, select **Product** > **Set up** > **Dimension groups**.

:::image type="content" source="./media/create-a-product/dimension-groups-setup.png" alt-text="Product menu in the Action Pane with the Dimension groups option in the Set up section.":::

1. In **Storage dimension group**, select **SiteWH**.
1. In **Tracking dimension group**, select **None**.
1. Select **OK**.
1. In the Action Pane, select **Release products**.
1. On the first page of the wizard, confirm that the step is **Select products to release**.

:::image type="content" source="./media/create-a-product/release-products-wizard.png" alt-text="Release products wizard showing the Select products to release step.":::

1. Select **Next**.
1. On **Select companies to release to**, select **USMF**.
1. Select **Next**.
1. On **Confirm selection**, set **Show Infolog upon failure** to **Yes** and **Run as batch** to **No**.
1. Select **Finish**.
1. In the navigation pane, select **Modules** > **Product information management**. Then, on the **Products** menu, select **Released products**.
1. On the **Released products** page, locate **GTL007**.
1. Select the product link to open the **Product details** page.
1. On the **General** FastTab, set **Item model group** to **FIFO**.
1. On the **Purchase** FastTab, set these values:
    - **Unit**: ea
    - **Item sales tax group**: ALL
    - **Price**: 30
1. On the **Sell** FastTab, set these values:
    - **Unit**: ea
    - **Item sales tax group**: ALL
    - **Price**: 35
1. On the **Manage inventory** FastTab, set **Unit** to **ea**.
1. On the **Engineer** FastTab, set **BOM Unit** to **ea**.
1. On the **Manage costs** FastTab, set **Item group** to **audio**.
1. To complete the configuration, in the Action Pane select **Product** > **Maintain** > **Validate**.

:::image type="content" source="./media/create-a-product/validate-product-action.png" alt-text="Product action pane showing the Validate command in the Maintain section.":::

1. Verify that an information banner appears and confirms that all required field values are valid.

:::image type="content" source="./media/create-a-product/validation-success-banner.png" alt-text="Information banner confirming that the product field values were validated successfully.":::

1. Close all pages, and then return to the home page.
