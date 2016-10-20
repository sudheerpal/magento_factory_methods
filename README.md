# magento_factory_methods

### Magento by default provides some of the really helpful factory methods to tweak the ecommerce system. 

Lets say, you want to get a collection of products which are prices between INR 100-200 and have inventory more than 10.
Making a SQL query and fetching information from complex EAV ( entity attributes values ) tables is definately a very sophisticated and complex task which every programmer know but know will like to do that.

Magento knows every ecommerce requirement and thus provides a very easy solution to this requirement.

#### Have a look to below code which seems to be self explanatory.


```php

 $_product = Mage::getModel('catalog/product')->load($_productID);
// loads an obejct with all properties of a product with given productID.

echo $_product->getName();
//prints the name of the product.

echo $_product->getShortDescription();
// similary this prints the short Description of products.

/* Similarly we can print all the attributes of a certain product, 
in case if you dont know attribute code then refer magento admin backend 
(catalog->attribute->manage attributes then search for the attribute code you are looking for. */

```
#### In case if you are looking for collection of more than one product, 
