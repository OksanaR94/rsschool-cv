# **Resume**

1. Antonova Oksana
1. ### My contact:  
    **phone:** +79277081869  
    **email:** Oksana.Rytova@yandex.ru  
1. *Good afternoon. My name's Oksana.* I began to study html and css for writing a graduation work in the last year of university. I created some simple sites after university for practics. My current job is not related to site development, but now I understood that I want to switched career and work a web developer. I know that I will have to work hard for improving my skills.
And I will try to accomplish my goal.
1. ### My Skills:
   * HTML, CSS
   * SQL, PL\SQL
   * ORACLE, PostgreSQL
   * PHP
   * Bootstrap

1. ### Code examples:  
  * product output
```
<div id="block-tovar-grid">
<?php
$resault  = pg_query($link,"SELECT * FROM table_products  limit $num offset $start");
if (pg_num_rows($resault) > 0)
{  $row = pg_fetch_array($resault);
    do{
      if ($row["image"] != "" && file_exists("./uploads_img/".$row["image"]) ) 
      {
        $img_path = './uploads_img/'.$row["image"];
        $max_width = 200;
        $max_height = 200;
        list($width, $height)= getimagesize($img_path);
        $ratioh = $max_height/ $height;
        $ratiow =  $max_width/$width;
        $ratio = min($ratioh,$ratiow);
        $width = intval($ratio*$width);
        $height = intval($ratio*$height);
      }else
      {
        $img_path = './images/no-image.png';
        $width = 110;;
        $height = 110;
      } 
        echo '
        <li><div class="block-images-grid" > 
        <img src="'.$img_path.'" width="'.$width.'" height="'.$height.'" /></div>
        <p class="style-title-grid"><a href=""> '.$row["title"].'  </a> </p>
        <a  class="add-cart-style-grid" >
        <form  metod="get" action="include/addtocart.php">
        <input type="submit" name="d_submit" id="d_submit" value="'.$row['products_id'].'" /></form>
        </a>
        <p class="style-price-grid"><strong> '.$row["price"].'</strong></p>
        </li> ';;
    }
    while ($row  = pg_fetch_array($resault) );
}
</div>
```  
  * Form registration 

```
div id="block-form-registration">
<ul id="form-registration">
<li>
<label>Login</label>
<input type="text" name="reg_login" id="reg_login" />
</li>
<li>
<label>Password</label>
<input type="text" name="reg_pass" id="reg_pass" />
</li>
<li>
<label>Surname</label>
<input type="text" name="reg_surname" id="reg_surname" />
</li>
<li>
<label>Name</label>
<input type="text" name="reg_name" id="reg_name" />
</li>
<li>
<label>E-mail</label>
<input type="text" name="reg_email" id="reg_email" />
</li>
<div>
<input type="checkbox" name="reg_checkbox" id="reg_checkbox"  />
<p id="fz">Я даю согласие на обработку моих персональных данных в соответсвии с ФЗ-152 "О персональных данных"</p>
</div>
</ul>
<p align="right"><input type="submit" name="reg_submit" id="form_submit" value="registration"/></p>
</div>
</form>
```
1. My projects  lists in group in vk. I created it during the period from 2016 to 2017.  For example some  simple sites - s cold-storage maintenance, home renovation. My graduation work is  
online store developmentstore.  
[Link of group:](https://vk.com/website_create_samara)    

1. 

1. 




