Magento Daily Deal Extension
======

Magento Configuration
-----------------------
In System > Configuration > Developer > Template Settings > Allow Symlinks, change to "Yes"

Display on Home Page
-----------------
Include the following code in Layout Update XML:
```xml
<reference name="content">
    <block type="dailydeal/deals" name="deals" template="dailydeal/browse.phtml">
        <block type="dailydeal/deal_list" name="deal_list" template="dailydeal/deal/list.phtml">
        </block>
    </block>
</reference>
```
Deal fields
-----------------
`Deals expire at` - time when deals expire  
`Number of daily deals` - the maximum number of deals available daily. Default is 3  
`URL Prefix` - the url for the deals section. Default is daily-deals  
`Deals manager email` - (todo) email of the person responsible for deals management. Used for reminders  
`Default deal quantity` - (todo) default quantity of products available in a deal. Can be overriden when creating a new deal  

Daily Deals Admin 
-----------------
* View/Create deals under Promotions => Daily Deals
* To caeate a deal, click "Add Daily Deal"
* In the Product Selection grid, select the product for the deal. Use name, sku, price etc filters to look for the products and press Search. Click on the product to select it
* Once product is selected, modify the Deal Settings as required. 

>>>>>>>>> Get <a href="http://magehit.com/magento-daily-deal-extension.html">Daily deal extension for Magento</a>
