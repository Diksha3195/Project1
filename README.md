# Project1
simple_project
Author:Diksha Bhingare
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>sidebar </title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.css"
    integrity="sha512-imTMcrMfwTWMwbgH3ComWWGCoDCo2jO1Qrvoa7B/Kcy7MrP5XMojK/Ede5uYofzcYyx4aFXdwzsm1QxdQXZreg=="
    crossorigin="anonymous" referrerpolicy="no-referrer" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"
    integrity="sha512-Avb2QiuDEEvB4bZJYdft2mNjVShBftLdPG8FJ0V7irTLQ8Uo0qcPxh4Plq7G5tGm0rU+1SPhVotteLpBERwTkw=="
    crossorigin="anonymous" referrerpolicy="no-referrer" />

  <link rel="stylesheet" href="style.css">
</head>

<body>
  <div class="main_box">
    <input type="checkbox" id="check" />
    <div class="btn_one">
      <label for="check">
        <i class="fa-solid fa-plus"></i>



      </label>
    </div>

    <div class="sidebar_menu">
      <div class="logo">
        <a href="#">Switch Plus</a>
      </div>

      <div class="btn_two">
        <label for="check" style="color: grey">

          <i class="fa-solid fa-x"></i>
        </label>
      </div>

      <div class="menu">
        <ul>
          <li>
            <i class="fa-solid fa-user"></i>
            <a href="#">Product</a>
          </li>
          <li>
            
            <i class="fa-regular fa-clipboard"></i>
            <a href="#">Book a Demo</a>
          </li>
          <li>
            
            <i class="fa-solid fa-phone"></i>

            <a href="#">Contact Us</a>
          </li>
          <li>
            
            <i class="fa-solid fa-store"></i>
            <a href="#">Store Locator</a>
          </li>
          <li>
            <i class="fa-regular fa-envelope-open"></i>
            <a href="#">Support</a>
          </li>
          <li>
            <i class="fa-regular fa-newspaper"></i>
            <a href="#">Career</a>
          </li>

        </ul>
      </div>

      <div class="social_media">
        <ul>
          <a href="#"><i class="fa-brands fa-facebook"></i></i></a>
          <a href="#"><i class="fa-brands fa-twitter"></i></a>
          <a href="#"><i class="fa-brands fa-instagram"></i></i></a>
          <a href="#"><i class="fa-brands fa-youtube"></i></a>
        </ul>
      </div>
    </div>
  </div>
</body>

</html>




style.css
*{
    margin: 0;
    padding: 0;
    font-family: Arial, Helvetica, sans-serif;
  
}
.main_box{
    background-image: url(photo.jpg);
    height: 100vh;
    background-size: cover;
    

}


.btn_one i{
    color: white;
    font-size: 25px;
    font-weight: 500;
    position: absolute;
    left: 10px;
    line-height: 60px;
    cursor: pointer;
    transition: all 2s linear;
    z-index: 100;
    
}
.sidebar_menu{
    position: fixed;
    left:-300px;
    height: 100vh;
    width: 300px;
    background-color: rgba(255, 255,255, 0.1);
    box-shadow: 0 0 5px rgba(255, 255,255, 0.5);

}
.sidebar_menu.logo{
    position: absolute;
    width: 100%;
    line-height: 80px;
    box-shadow: 0 0 6px rgba(255, 255,255, 0.5);
    height: 60px;


}
.logo a{
    position: absolute;
    top: 15px;
    left: 70px;
    color: white;
    width: 100%;
    font-size: 25px;
    font-weight: 700;
    text-decoration: none;
    
    

}
.logo{
    box-shadow: 0 0 5px rgba(255, 255,255, 0.5);
}
.btn_two i{
    position: absolute;
    color: gray;
    font-size: 20px;
    font-weight: 700;
    left: 270px;
    top: 15px;
    opacity: 1;
    cursor: pointer;
   

}
.menu{
    margin-top: 100px;
    position: absolute;
    width: 100%;
    color: white;
    
    
}
.menu li{
    margin-top: 8px;
    padding: 10px 20px ;
}
.menu i,a{
    color: white;
    font-size: 20px;
    font-weight: 500;
    text-decoration: none;
}
.menu i{
    padding-right: 10px;
}
.social_media{
    position: absolute;
   
    left: 25%;
    bottom: 50px;

}
.social_media i{
    color: white;
    opacity: 0.5;
    padding: 5px;
}
#check{
    display:none;
}
.menu li:hover{
    box-shadow: 0 2px rgba(255, 255,255, 0.5);
}
.btn_one i:hover{
    font-size: 30px;
}
.btn_two i:hover{
    font-size: 30px;
   
}
.social_media i:hover{
    opacity: 1;
    transform: scale(1.1);

}

#check:checked~ .sidebar_menu{

    left: 0;
}
#check:checked~ .btn_one{
    opacity: 0;
}
#check:checked~ .sidebar_menu.btn_two{
    opacity: 1;
}



