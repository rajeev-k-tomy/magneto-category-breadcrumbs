magneto-category-breadcrumbs
============================

INTRODUCTION
---------------
This module allow us to add breadcrumbs only for category pages. It will remove breadcrumbs from all other pages except category page. 

The idea for the extension came from here http://stackoverflow.com/questions/25201927/magento-breadcrumbs-on-category-page/. 

In order to make it fully functional, you want to call my breadcrumbs extension in your current category view page

    File : app/design/frontend/<your_package>/<your_theme>/template/catalog/cateogry/view.phtml
    
    <div><?php echo $this->getChildHtml('category_breadcrumbs'); ?></div>
    
  COMPATIBILITY
  ----------------
  
  I have tested it only in Magento 1.8 . But most probably it will work with any version.
  
  PRO
  -----
  
It does not contain any rewrite  to core files

It does not touch any core files

It does not use any observers

 CONS
 -----------
 
 As I already mentioned, you need to call my `breadcrumbs block` manually in your `category view page`.
 
 THEORY
 -------
 
 I have well expalined the theory concept in this stack over flow link http://stackoverflow.com/questions/25201927/magento-breadcrumbs-on-category-page/ .  Please make a look
 
