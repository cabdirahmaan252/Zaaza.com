<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Zaaza Page</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
  <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: Poppins, sans-serif;
      background-color: white;
      width: 100%;
      overflow-x: hidden;
    }

    header.container {
      display: flex;
      width: 100%;
      background-color:#fff;
      justify-content: space-between;
      align-items: center;
      padding: 0.5rem;
    /*  padding: 10px 15px;*/
      position: fixed;
      z-index: 999;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 1rem;
      justify-content: flex-end;
      align-items: center;
    }

    nav a {
      font-size: 1.1em;
      text-decoration: none;
      font-weight: 500;
      color: #4e6cff;
    }
    nav a:hover{
      color: purple;
    }

    /* Hide the toggle button by default */
    .menu-toggle {
      display: none;
      margin-left: auto;
      font-size: 1.8rem;
      color: #111;
      cursor: pointer;
    }
    .Logo a{
      text-decoration: none;
      font-size: 1.7em;
      font-weight: 700;
      color: #4e6cff;
      cursor: none;
      text-transform: uppercase;
    }
    section{
      widoth: 100%;
      max-width: 1600px;
      text-align: left;
      padding-bottom: 2.5em;
     /* padding-bottom: 40px;*/
      padding-top: 10px;
    }
    .main{
      width: 100%;
      margin-top: 3.75em;
      background: url("266ec5ffbf5bdbf0902b54a66a9ab483(Copy).jpg") no-repeat;
      background-attachment: fixed;
      position: center;
      background-size: cover;
    }
    .main h2 {
      margin-left: 1.25em;
      color: white;
      margin-top: 1.875em;
      font-size: 1.4em;
      font-weight: 500;
    }
    .main h2 span{
      color: white;
      display: inline-block;
      color: orange;
      margin-top: 0.625em;
      font-size: 3em;
      font-weight: 600;
    }
    .main h3 {
      color: white;
      margin-left: 1.25em;
      font-size: 2rem;
      font-weight: 700;
      margin-top: 0.625em;
      margin-bottom: 1.875em;
      base-palette: 0.0625em;
    }
    .main-btn {
      text-decoration: none;
      display: inline-block;
      margin-bottom: 1.875em;
      color: white;
      font-size: 1.3em;
      font-weight: 600;
      background-color: #4e6cff;
      border-radius: 0.9375em;
      margin-left: 1.25em;
      padding: 0.9375em;
      transition: 0.7s ease;
    }
    .main-btn:hover{
      background-color: #0a49f6;
      transform: scale(1.1);
    }
    .social-icons a{
      text-decoration: none;
      margin-left: 1.25em;
      color: white;
      font-size: 2em;
      font-weight: 600;
      padding-left: 0.625em;
    }
    .title{
      display: flex;
      justify-content: center;
      color: #4c6eff;
      margin: 20px;
    }
    .content{
      width: 100%;
      display: flex;
      justify-content: center;
      padding: 25px;
      flex-direction: row;
      flex-wrap: wrap;
      text-align: center;
    }
    .card{
      background-color: #fff;
      width: 21.25em;
      padding: 25px;
      font-size: 1em;
      box-shadow: 0 5px 25px rgba(1 1 1/25);
      border-radius: 15px;
      margin: 15px;
      transition: 0.7s ease;
    }
    .name{
      font-size: 1em;
      font-weight: 800;
      color: #4c6eff;
      margin-bottom: 20px;
    }
    .icon{
      font-size: 4rem;
      text-align: center;
      color: black;
      margin-bottom: 20px;
    }
    .card:hover{
      transform: scale(1.1);
    }
    .pragraph{
      letter-spacing: 1px;
    }
    main{
      width: 100%;
      text-align: left;
      padding-bottom: 40px;
      padding-top: 10px;
    }
    
    main p{
      letter-spacing: 1px;
      text-align: center;
      font-size: 1em;
    }
    .definition{
      padding-bottom: 20px;
      font-size: 1.5em;
      font-weight: 600;
    }
    main ul {
      list-style: none;
      letter-spacing: 2px;
      padding: 20px;
    }
    main li {
      padding: 5px 0 ;
    }
    form{
      width: 100%;
      background-color: #fff;
      width: 30em;
      padding: 25px;
      font-size: 1em;
      box-shadow: 0 5px 25px rgba(1 1 1/25);
      border-radius: 15px;
      margin: 15px;
      margin-left: 255px;
    }
    .Contact-icon{
      display: flex;
      gap: 1rem;
      color: black;
      margin-bottom: 4px;
    }
    .Contact-icon a{
      color: black;
      text-decoration: none;
      font-size: 1.2em;
    }
    .Contact-icon i{
      font-size: 1.7em;
    }
    form h3{
      font-size: 1.2em;
      font-weight: 800;
      margin-bottom: 20px;
    }
    /* Responsive styles */
    @media (max-width: 501px) {
      .menu-toggle {
        display: block;
      }

      nav ul {
        display: none;
        flex-direction: column;
        align-items: flex-end;
        background-color: #333;
        padding: 50px 50px;
        position: absolute;
        top: 70px;
        height: 100vh;
        justify-content: center;
        text-align: center;
        align-items: center;
        right: -450px;
        width: 200px;
        border-radius: 10px 0 0 10px;
        transition: right 3s ease;
        z-index: 100;
      }

      nav ul.show {
        display: flex;
        right: 0;
      }

      nav a {
        color: white;
        text-align: center;
        display: block;
        width: 100%;
        padding:0px;
      }
      
    .main{
      background: url("266ec5ffbf5bdbf0902b54a66a9ab483.jpg") no-repeat;
      background-attachment: fixed;
      position: center;
      background-size: cover;
      max-height:95vh;
    }
    
    .main h2 {
      margin-left: 20px;
      color: white;
      margin-top: 30px;
      font-size: 1.1em;
      font-weight: 500;
    }
    
    .main h2 span{
      color: white;
      display: inline-block;
      color: orange;
      margin-top: 10px;
      font-size: 2em;
      font-weight: 800;
    }
    
    .main h3 {
      color: white;
      margin-left: 20px;
      font-size: 1.7rem;
      font-weight: 700;
      margin-top: 10px;
      margin-bottom: 30px;
      base-palette: 1px;
    }
    
    .main-btn {
      text-decoration: none;
      display: inline-block;
      margin-bottom: 30px;
      color: white;
      font-size: 1em;
      font-weight: 600;
      background-color: #4e6cff;
      border-radius: 15px;
      margin-left: 20px;
      padding: 15px;
      transition: 0.7s ease;
    }
    
    .main-btn:hover{
      background-color: #0a49f6;
      transform: scale(1.1);
    }
    .social-icons a{
      text-decoration: none;
      margin-left: 20px;
      color: white;
      font-size: 1.5em;
      font-weight: 600;
      padding-left: 0px;
    }
    
    .title{
      display: flex;
      justify-content: center;
      color: #4c6eff;
      margin: 15px;
    }
    .content{
      display: flex;
      justify-content: center;
      padding: 15px;
      flex-direction: row;
      flex-wrap: wrap;
      text-align: center;
    }
    .card{
      background-color: #fff;
      width: 20em;
      padding: 20px;
      font-size: 1em;
      box-shadow: 0 5px 25px rgba(1 1 1/25);
      border-radius: 15px;
      margin: 15px;
      transition: 0.7s ease;
    }
    .name{
      font-size: 1em;
      font-weight: 800;
      color: #4c6eff;
      margin-bottom: 20px;
    }
    .icon{
      font-size: 5rem;
      text-align: center;
      color: black;
      margin-bottom: 20px;
    }
    .card:hover{
      transform: scale(1.1);
    }
    .pragraph{
      letter-spacing: 1px;
    }
    main{
      width: 100%;
      text-align: left;
      padding-bottom: 40px;
      padding-top: 10px;
    }
    
    main p{
      letter-spacing: 1px;
      text-align: center;
      font-size: 0.9em;
    }
    .definition{
      padding-bottom: 20px;
      font-size: 1em;
      font-weight: 600;
    }
    main ul {
      list-style: none;
      letter-spacing: 2px;
      padding: 20px;
    }
    main li {
      padding: 5px 0 ;
    }
    form{
      background-color: #fff;
      width: 20em;
      padding: 20px;
      font-size: 1em;
      box-shadow: 0 5px 25px rgba(1 1 1/25);
      border-radius: 15px;
      margin: 15;
      margin-left: 85px;
      transition: 0.7s ease;
    }
    .Contact-icon{
      display: flex;
      gap: 1rem;
      color: black;
      margin-bottom: 4px;
    }
    .Contact-icon a{
      color: black;
      text-decoration: none;
      font-size: 1.2em;
    }
    .Contact-icon i{
      font-size: 1.7em;
    }
    form h3{
      font-size: 1.2em;
      font-weight: 800;
      margin-bottom: 20px;
    }
    }
    @media (max-width: 370px) {
      .menu-toggle {
        display: block;
      }

      nav ul {
        display: none;
        flex-direction: column;
        align-items: flex-end;
        background-color: #333;
        padding: 50px 50px;
        position: absolute;
        top: 95px;
        right: -250px;
        width: 200px;
        border-radius: 10px 0 0 10px;
        transition: right 0.3s ease;
        z-index: 100;
      }

      nav ul.show {
        display: flex;
        right: 0;
      }

      nav a {
        color: white;
        text-align: center;
        display: block;
        width: 100%;
        padding:0px;
      }
    .main{
      background: url("266ec5ffbf5bdbf0902b54a66a9ab483.jpg") no-repeat;
      background-attachment: fixed;
      position: center;
      background-size: cover;
    }
    .main h2 {
      margin-left: 20px;
      color: white;
      margin-top: 30px;
      font-size: 1.1em;
      font-weight: 500;
    }
    .main h2 span{
      color: white;
      display: inline-block;
      color: orange;
      margin-top: 10px;
      font-size: 2em;
      font-weight: 800;
    }
    .main h3 {
      color: white;
      margin-left: 20px;
      font-size: 1.7rem;
      font-weight: 700;
      margin-top: 10px;
      margin-bottom: 30px;
      base-palette: 1px;
    }
    .main-btn {
      text-decoration: none;
      display: inline-block;
      margin-bottom: 30px;
      color: white;
      font-size: 1em;
      font-weight: 600;
      background-color: #4e6cff;
      border-radius: 15px;
      margin-left: 20px;
      padding: 15px;
      transition: 0.7s ease;
    }
    .main-btn:hover{
      background-color: #0a49f6;
      transform: scale(1.1);
    }
    .social-icons a{
      text-decoration: none;
      margin-left: 20px;
      color: white;
      font-size: 1.5em;
      font-weight: 600;
      padding-left: 0px;
    }
    
    .title{
      display: flex;
      justify-content: center;
      color: #4c6eff;
      margin: 15px;
    }
    .content{
      display: flex;
      justify-content: center;
      padding: 15px;
      flex-direction: row;
      flex-wrap: wrap;
      text-align: center;
    }
    .card{
      background-color: #fff;
      width: 20em;
      padding: 20px;
      font-size: 1em;
      box-shadow: 0 5px 25px rgba(1 1 1/25);
      border-radius: 15px;
      margin: 15px;
      transition: 0.7s ease;
    }
    .name{
      font-size: 1em;
      font-weight: 800;
      color: #4c6eff;
      margin-bottom: 20px;
    }
    .icon{
      font-size: 5rem;
      text-align: center;
      color: black;
      margin-bottom: 20px;
    }
    .card:hover{
      transform: scale(1.1);
    }
    .pragraph{
      letter-spacing: 1px;
    }
    main{
      width: 100%;
      text-align: left;
      padding-bottom: 40px;
      padding-top: 10px;
    }
    
    main p{
      letter-spacing: 1px;
      text-align: center;
      font-size: 0.9em;
    }
    .definition{
      padding-bottom: 20px;
      font-size: 1em;
      font-weight: 600;
    }
    main ul {
      list-style: none;
      letter-spacing: 2px;
      padding: 20px;
    }
    main li {
      padding: 5px 0 ;
    }
    form{
      background-color: #fff;
      width: 13em;
      padding: 15px;
      font-size: 1em;
      box-shadow: 0 5px 25px rgba(1 1 1/25);
      border-radius: 15px;
      margin: 15;
      margin-left: 20px;
      transition: 0.7s ease;
    }
    .Contact-icon{
      display: flex;
      gap: 1rem;
      color: black;
      margin-bottom: 4px;
    }
    .Contact-icon a{
      color: black;
      text-decoration: none;
      font-size: 1.2em;
    }
    .Contact-icon i{
      font-size: 1.7em;
    }
    form h3{
      font-size: 1.2em;
      font-weight: 800;
      margin-bottom: 20px;
    }
    }
  </style>
</head>
<body>
  <header class="container">
    <div class="Logo">
      <img src="20250614_055048.png" height="60">
    </div>
    <div class="menu-toggle" onclick="toggleMenu()">
      <i class="fas fa-bars"></i>
    </div>
    <nav>
      <ul id="nav-links">
        <li><a href="#Services">Services</a></li>
        <li><a href="#Contact">Contact</a></li>
        <li><a href="#about-me">About me</a></li>
      </ul>
    </nav>
  </header>
  <hr>
 <section class="main">
   <h2>Hi i'm abdi rahman <br> <span>Web developer</span></h2>
   <h3>I buil front-end website</h3>
   <a href="#" class="main-btn" onclick="showMessage()">View my works</a>
   <div class="social-icons">
     <a href="https://wa.me/252617402662" target="_blank"><i class="fa-brands fa-whatsapp"></i></a>
     <a href="https://www.facebook.com/share/16gKt2tZ9S/" target="_blank"><i class="fa-brands fa-facebook"></i></a>
     <a href="https://x.com/MAHADCABDI252?s=09" target="_blank"><i class="fa-brands fa-x-twitter"></i></a>
   </div>
 </section>
 <section class="Services" id="Services">
   <h2 class="title">Services</h2>
   <div class="content">
     <div class="card">
       <div class="icon">
         <i class="fa-solid fa-desktop"></i>
       </div>
       <div class="name">
         <h3>Full responsive</h3>
       </div>
       <div class="pragraph">
         <p>waxa ku sameey karaa website page leh Responsive oo ku shaqeeya dhammaan aaladaha kala duwan</p>
       </div>
     </div>
     <div class="card">
       <div class="icon">
         <i class="fa-solid fa-pen-to-square"></i>
       </div>
       <div class="name">
         <h3>Code edit</h3>
       </div>
       <div class="pragraph">
         <p>Haddii aad rabto inaad wax ka beddesho koodka, waxaan ku siinayaa adeegga wax ka beddelka qaladaadka koodka.</p>
       </div>
     </div>
   </div>
 </section>
 <hr>
 <main class="about-me" id="about-me">
   <h2 class="title">About me</h2>
   <p class="definition">
     <strong>Freelancer – Front-End Developer (Basic Level)</strong>
   </p>
   <p>
     Hi! I'm Cabdi Raxmaan, a passionate Front-End Developer with a focus on creating clean, responsive, and user-friendly websites.
   </p>
   <p>
     I specialize in building landing pages and simple websites using:
   </p>
   <p>
     <ul>
       <li>✅ HTML & CSS</li>
       <li>✅ JavaScript (basic functionality)</li>
       <li>✅ Bootstrap or Tailwind CSS (upon request)</li>
       <li>✅ Fully responsive (mobile, tablet & desktop)</li>
     </ul>
   </p>
 </main>
 <hr>
 <main>
    <h2 class="title" id="Contact">Contact</h2>
    <form>
      <h3>Contact me here</h3>
      <div class="Contact-icon">
        <a href="https://wa.me/252617402662"target="_blank" class="Contact-icon">
          <i class="fa-brands fa-whatsapp"></i>
        </a>
        <a href="https://wa.me/252617402662" target="_blank">whatsapp</a>
      </div>
      <div class="Contact-icon">
        <a href="https://www.facebook.com/share/16gKt2tZ9S/"target="_blank" class="Contact-icon">
          <i class="fa-brands fa-facebook"></i>
        </a>
        <a href="https://www.facebook.com/share/16gKt2tZ9S/" target="_blank">facebook</a>
      </div>
      <div class="Contact-icon">
        <a href="https://x.com/MAHADCABDI252?s=09"target="_blank" class="Contact-icon">
          <i class="fa-brands fa-x-twitter"></i>
        </a>
        <a href="https://x.com/MAHADCABDI252?s=09" target="_blank">twitter</a>
      </div>
      <div class="Contact-icon">
        <a href="https://www.instagram.com/nedvedo1?igsh=MWx5c3EzMmQ4cm1xOQ=="target="_blank" class="Contact-icon">
          <i class="fa-brands fa-instagram"></i>
        </a>
        <a href="https://www.instagram.com/nedvedo1?igsh=MWx5c3EzMmQ4cm1xOQ==" target="_blank">instegram</a>
      </div>
    </form>
  </main>
  <script>
    function toggleMenu() {
      const navLinks = document.getElementById('nav-links');
      navLinks.classList.toggle('show');
    }
    function showMessage(){
      alert("wali wax xog ah lama soo gelin")
    }
  </script>
  <footer style="text-align:center; padding: 60px; background:#4e6cff; color:white;">
  <p>© 2025 Zaaza - All Rights Reserved</p>
</footer>
</body>
</html>
