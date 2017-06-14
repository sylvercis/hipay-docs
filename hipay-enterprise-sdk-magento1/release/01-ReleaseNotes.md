# Release notes


## v1.7.0

**Publish date** : 06-12-2017  
[*GitHub Release*](https://github.com/hipay/hipay-fullservice-sdk-magento1/releases/tag/1.7.0)


* New - Oney Facily Pay support  
*Oney Facily Pay 3X and 4X with fees or no fees*

* New - Astropay support  
*We add severals payment methods for Mexico and Brazil.
The module now supports :*
  * *Oxxo*
  * *Aura*
  * *Caixa*
  * *BBVA Bancomer*
  * *Santader cash*
  * *Bradesco*
  * *Boleto*
  * *Itau*


* New - Mapping yours categories with HiPay  
* New - Mapping yours shipping methods with HiPay and determine delivery date  
*Two new screens are available for mapping your categories and your shipping method with the HiPay data. These screens are available in the general configuration of the Hipay module.
This mapping is mandatory for Oney Facily Pay*

##v1.6.2

**Publish date** : 05-05-2017  
[*GitHub Release*](https://github.com/hipay/hipay-fullservice-sdk-magento1/releases/tag/1.6.2)

* Fix - Domain TokenJS  
*The url for hipay tokenization was per defaut on production.*

##v1.6.1

**Publish date** : 04-13-2017  
[*GitHub Release*](https://github.com/hipay/hipay-fullservice-sdk-magento1/releases/tag/1.6.1)

Fix - [SECURITY] Check notification signature if passphrase is not empty  
Fix - X-forward-for without proxy  
Fix - Http code if signature is wrong  

##v1.6.0

**Publish date** : 02-23-2017  
[*GitHub Release*](https://github.com/hipay/hipay-fullservice-sdk-magento1/releases/tag/1.6.0)

New - Payment MO/TO configuration
New - Payment MO/TO send to customer the payment page link
New - New Branding HiPay
New - New order_id nomenclature on the split payment
New - Optimization the split payment profil labels
New - Add Request sources send to the request API
New - Change "Hipay's Cards" title
New - Basket configuration
New - Basket: Send the basket to transaction
New - Basket: Available to capture and refund
New - Additional parameters: use order currency to transaction
New - Payment method: add Klarna integration associated with the basket feature
New - Changing Payment Methods at Store View in addition to the general config
Fix - tax-rate to the split payment
Fix - The cancel management by the back office HiPay towards Magento
Fix - Callback 142 Authorization requested
Fix - Custom_data file is on error when it's not used


