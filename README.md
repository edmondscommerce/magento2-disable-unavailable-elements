# Magento 2 Disable Unavailable Elements
## By [Edmonds Commerce](https://www.edmondscommerce.co.uk)

Prevents a user from clicking on page elements before they're fully loaded

### Default targets

The following elements are targeted by the module:

- Hamburger menu
- Header search icon
- Shop by button
- Category sorter
- Product add to cart form
- Cart discount block
- Cart proceed button
- Header language switcher

The overlay is applied as long as the `body` element does not have `aria-busy="false"`.

See `view/frontend/web/css/source/_module.less` for more details.

### Adding your own elements

Use these mixins in your theme to add elements to the list of items to be disabled during page load. 

You can either use them as Less mixins, or add and remove these classes using Javascript. 

- `.loading-disabled;` - This provides an indication that the item is loading
- `.loading-click-block;` - This adds a transparent overlay to prevent clicks
 

