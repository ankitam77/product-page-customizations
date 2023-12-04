# Product Page Customization

This project is for mainly focusing on Shopify Online 2.0 and 3.0 features. Online Store 2.0 opens up massive opportunities for developers building themes and apps for Shopify merchants. There are many features which are introduced in shopify online store 2.0, including
 * Shopify Theme Architecure
 * Metafields Massive changes
 * Theme Editor Enhancements
 * Development Tools (mainly CLI)
 * Github Integration with shopify store
Recently, Shopify has also introduced Online store 3.0. Some of the feature are introduced including
 * Workflow changes
 * Metaobjects
We are trying to customize the product page with the above mentioned changes where we have created metaobjects to display structured data for product page. Metaobjects use **metafields** to store their fields. We have focused on creating custom section which can be used on any type of pages.

# Installation

## Prerequisites

1. You must [create a Shopify partner account] (https://partners.shopify.com/signup) if you don’t have one.
2. You must create a store for testing if you don't have one, [a development store](https://help.shopify.com/en/partners/dashboard/development-stores#create-a-development-store)

## Steps to install

1. **[Download Zip folder](https://github.com/ankitam77/product-page-customizations/archive/refs/heads/main.zip)**
2. Login to admin portal of Shopify store (Assuming you have created if you don't have).
3. Once logged in, Go to Sales Channel -> Online Store -> Themes.
4. Click on Add Theme under Theme Library. Click on Upload Zip File.
5. Once uploaded the theme, you can publish the theme or you can preview the theme.

 ## Adding data to store

We need to add products, collections, page data to store along with metaobjects and metafield. We will be using [metrixify](https://apps.shopify.com/excel-export-import) app to import data. Please  make sure that you installed this app on your store.
Before importing data to store, we need to create definations for metaobjects and metafields. There is no way to import metafields and metaobjects without creating definations in targeted store. 

To create definations, please go through below steps.

 1. **Create defination for metaobjects:**


   * In Shopify Admin, go to Settings-> Custom Data -> Metaobjects. Click on **Add Defination**.
     
    <img width="772" alt="image" src="https://github.com/ankitam77/product-page-customizations/assets/94292839/4f9fc398-5b98-47f8-a614-d51dd0707273">


   * Add "Product Specifications" in Name input field.
   * Click on Add Field. Select Single Line Text. Add Name "Heading". Check the checkbox of 'Display Name'. Keep selected One Value. Click on Add. This is only for purpose to make sure what value is going to use for what data. This will not get displayed on storefront.
   * Click on Add Field. Select Single Line Text. Add Name "Sleeve Length". Keep selected One Value. Click on Add.
   * Click on Add Field. Select Single Line Text. Add Name "Neck". Keep selected One Value. Click on Add.
   * Click on Add Field. Select Single Line Text. Add Name "Length". Keep selected One Value. Click on Add.
   * Click on Add Field. Select Single Line Text. Add Name "Pattern". Keep selected One Value. Click on Add.
   * Click on Add Field. Select Single Line Text. Add Name "Type". Keep selected One Value. Click on Add.
   * Click on Add Field. Select Single Line Text. Add Name "Occasion". Keep selected One Value. Click on Add.
   * Save the metaobject defination.


2.  **Add a Metafield reference**


  To enable the dynamic content we need to add a metafield reference.


  * In Shopify Admin, go to Settings-> Custom Data -> Metafields -> Products. Click on **Add Defination**.
  * Add product metafield name "Product Specifications" in Name input field.
  * Select type -> Metaobjects -> Select referenece by seecting metaobjects.
    
    <img width="484" alt="image" src="https://github.com/ankitam77/product-page-customizations/assets/94292839/c0f5b0b7-1e39-4f5d-859a-bb0baf8434db">
    
  * Select List Of Entries and Save.


3. **Import store sample data**
   
  * Go to Apps -> Metrixify App.
  * Under Import Options 'Add File'. File is available in root folder with name 'custom-data.xls'.
  * Once added and ready to import, click on 'Import' button.
  * It will show the progress and also will generate report of importing data if successful or failed.
  * We have to be very pretty sure about the the file which we are importing, specifically for metafields and metaobjects. If any defination fails to match it will not   import the data.

4. YOu can check the metafields and metaobjects data which is added with products is displayed on product page under specifications.
5. 'Our Story' section is custom section which is displaying a page. We can change with any other page.


## Additional Information

We are not updating anything to cart functionlaity as all major functions are coming with theme itself. Below are those functions which are already there with latest theme:

1. Product is added to cart as soon as we click 'Add to cart' without refreshing page.
2. Increase or decrease the quantity of the items directly from the cart.
3. Remove items from the cart.
4. It prevents multiple submissions too.

We are always ready to take new challange. So if anything which is new and useful for cart functionality, we would be working on it. Please share you ideas for the same.



