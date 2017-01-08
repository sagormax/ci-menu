# ci-menu
Codeigniter Menu Library

# Instruction 
1.  First copy Menu.php file to your libraries directory.
2.  Open config >> autoload.php file and add this Menu library to library section 
    OR
    add this line to your controller.

    ```php
    $this->load->library('Menu');
    ```

3.  Generate menu on frontend

    ```php
    <?php
    $attr = array(
        'table_name'          => 'ci_menu',
        'menu_cat_ID'         =>  1,
        'ul_class'            => "",
        'ul_ID'               => "nav-main",
        'ul_attr'             => '',
        'li_class'            => "item-list",
        'li_if_submenu_after' => "<i class='fa fa-angle-down'></i>",
        'li_if_submenu_class' => "",
        'ul_submenu_class'    => "",
        'ul_submenu_ID'       => "secondary",
    );
    echo $this->menu->generateFrontendMenu($attr);
    ?>    
    ```