# Replace-Add-to-Cart-or-Add-to-Cart-
Replace “Add to Cart” or “Add to Cart”
/**
 * Change the add to cart text on single product pages
 */
function woo_custom_cart_button_text() {
        return __('My Button Text', 'woocommerce');
}
add_filter('single_add_to_cart_text', 'woo_custom_cart_button_text');
 
/**
 * Change the add to cart text on product archives
 */
function woo_archive_custom_cart_button_text() {
        return __( 'My Button Text', 'woocommerce' );
}
add_filter( 'add_to_cart_text', 'woo_archive_custom_cart_button_text' );
