1. From your Shopify admin, go to Online Store > Themes.
2. Find the theme you want to edit, and then click Actions > Edit code.
3. In the Layout directory, click theme.liquid.

4. Find the closing </body> tag. On a new line right above the closing </body> tag, paste the following code:

{% render 'ajax-cart.liquid' %}

5. Click Save.
6. In the Snippets directory, click Add a new snippet:

7. Name your snippet ajaxify-cart, and click Create snippet:

8. In your new ajaxify-cart.liquid file, paste this code hosted on ajax-cart.liquid this file.

Caution: In the pasted code, replace all instances of .size() with .length. The .size() method is depreciated as of JQuery 1.8.

9. Click Save.


10. In the same file {% render 'ajax-cart.liquid' %}, find the following code:

cartCountSelector: '.cart-count, #cart-count a:first, #gocart p a, #cart .checkout em, .item-count',

