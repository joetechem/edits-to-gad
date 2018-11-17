# edits-to-gad
throwaway repo to keep track of changes

***  
#### 1) Parse error: syntax error, unexpected T_PAAMAYIM_NEKUDOTAYIM, expecting T_VARIABLE in /home/content/38/7576538/html/greatamericandirect/wp-content/plugins/yith-woocommerce-wishlist/plugin-fw/lib/yit-plugin-panel.php on line 101  

#### yit-plugin-panel.php - Line 101:  
```php  
// original
static::_init_actions();

//change
static->_init_actions();
```  
***  

Fixing syntax beyond this brings up more syntax errors. I believe the bottom line is the server it is sitting on needs to have its PHP updated; otherwise, this could take months (manually updating --really downgrading-- all the PHP code, which is a lot). Currently it is running PHP 5.2, whereas our site we have migrated here has very recently updated plugins. --Need to revisit/possibly touch base with the client, to make sure the update to a newer PHP version does not break the other site they have. I don't think it will, as the code for the other site does not seem to be sitting here, just its domain. Will double-check first, as this environment is owned by client.


