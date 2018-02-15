
<?php

function my_account($content) {
	
	// if our current user is seller
	$is_seller=false;
	
	// get current user
	$user = wp_get_current_user();
	
	//if user role in array of $user roles
	if ( in_array( 'seller', (array) $user->roles ) ) {
		$is_seller=true;
	}
	
	// if this page is my-account and user is seller then 	
	if (is_page("my-account") && $is_seller==true){
		
		$content="[dokan-dashboard]";
	}
	
   return $content;

}
add_filter( 'the_content', 'my_account');

?>
