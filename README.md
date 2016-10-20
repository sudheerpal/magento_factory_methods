# magento_factory_methods

## Magento by default provides some of the really helpful factory methods to tweak the ecommerce system. 

Lets say, you want to get a collection of products which are prices between INR 100-200 and have inventory more than 10.
Making a SQL query and fetching information from complex EAV ( entity attributes values ) tables is definately a very sophisticated and complex task which every programmer know but know will like to do that.

Magento knows every ecommerce requirement and thus provides a very easy solution to this requirement.

#### Have a look to below code which seems to be self explanatory.


```php


 $_products = Mage::getModel('catalog/product')->load($_productID)
// loads an obejct with all properties of a product with given productID.



```
