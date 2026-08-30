<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Untuk Kamu❤️</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
      font-family: "Arial", sans-serif;
      background: linear-gradient(135deg, #ffb6c9, #ffe5ed, #fff);
    }

    /* =====================
       HATI JATUH
    ====================== */

    .heart {
      position: fixed;
      top: -20px;
      color: #ff5c8a;
      font-size: 20px;
      animation: fall linear forwards;
      pointer-events: none;
      z-index: 1;
    }

    @keyframes fall {
      to {
        transform: translateY(110vh) rotate(360deg);
        opacity: 0;
      }
    }

    /* =====================
       CARD
    ====================== */

    .card {
      position: relative;
      z-index: 5;
      width: 90%;
      max-width: 430px;
      max-height: 90vh;
      overflow: hidden;
      background: rgba(255,255,255,0.94);
      padding: 25px;
      text-align: center;
      border-radius: 30px;
      box-shadow: 0 15px 40px rgba(190, 70, 110, 0.25);
      backdrop-filter: blur(10px);
    }

    h1, h2 {
      color: #ff4778;
    }

    p {
      color: #555;
      line-height: 1.7;
    }

    /* =====================
       PASSWORD
    ====================== */

    #content {
      display: none;
    }

    input {
      width: 100%;
      padding: 14px;
      border: 2px solid #ffc0d0;
      border-radius: 15px;
      outline: none;
      text-align: center;
      font-size: 17px;
      margin: 15px 0;
    }

    button {
      border: none;
      background: linear-gradient(135deg, #ff4778, #ff7199);
      color: white;
      padding: 12px 22px;
      border-radius: 25px;
      cursor: pointer;
      font-size: 15px;
      margin: 5px;
      box-shadow: 0 5px 15px rgba(255,71,120,0.25);
      transition: 0.25s;
    }

    button:hover {
      transform: scale(1.05);
    }

    #error {
      display: none;
      color: #ff3b6b;
    }

    /* =====================
       SLIDE
    ====================== */

    .slide {
      display: none;
      animation: slideIn 0.6s ease;
    }

    .slide.active {
      display: block;
    }

    .slide img {
      width: 100%;
      height: 300px;
      object-fit: cover;
      border-radius: 22px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.12);
    }

    @keyframes slideIn {
      from {
        opacity: 0;
        transform: translateX(40px);
      }

      to {
        opacity: 1;
        transform: translateX(0);
      }
    }

    /* =====================
       DOT
    ====================== */

    .dots {
      margin-top: 10px;
    }

    .dot {
      display: inline-block;
      width: 9px;
      height: 9px;
      margin: 4px;
      border-radius: 50%;
      background: #ffc0d0;
    }

    .dot.active {
      background: #ff4778;
      transform: scale(1.3);
    }

    /* =====================
       MUSIK
    ====================== */

    .music {
      margin-bottom: 10px;
      font-size: 13px;
      color: #999;
    }

    /* =====================
       SLIDE TERAKHIR
    ====================== */

    .big-heart {
      font-size: 60px;
      animation: heartbeat 1.2s infinite;
    }

    @keyframes heartbeat {
      0%, 100% {
        transform: scale(1);
      }

      50% {
        transform: scale(1.2);
      }
    }

    #thanks {
      display: none;
      animation: fade 1s ease;
    }

    @keyframes fade {
      from {
        opacity: 0;
      }

      to {
        opacity: 1;
      }
    }
  </style>
</head>

<body>

  <!-- =========================
       PASSWORD
  ========================== -->

  <div class="card" id="login">

    <h1>🔐 Untuk Kamu❤️</h1>

    <p>
      Ada sesuatu yang ingin aku sampaikan...
    </p>

    <p>
      Masukkan password dulu ya sayang

    </p>

    <input
      type="password"
      id="password"
      placeholder="Password"
    >

    <br>

    <button onclick="checkPassword()">
      Buka❤️
    </button>

    <p id="error">
      Password salah kok bisa?
    </p>

  </div>


  <!-- =========================
       ISI UTAMA
  ========================== -->

  <div class="card" id="content">

    <div class="music">
      🎵 Musik untuk kamu
    </div>

    <audio id="music" loop>
      <source src="musik.mp3" type="audio/mpeg">
    </audio>


    <!-- SLIDE 1 -->

    <div class="slide active">

      <img src="IMG-20260817-WA0000.jpg" alt="Foto kita">

      <h2>Maaf cintaa❤️</h2>

      <p>
        Aku tahu aku sudah melakukan kesalahan.
        Dari lubuk hati yang paling dalam,
        aku benar-benar minta maaf.
      </p>

    </div>


    <!-- SLIDE 2 -->

    <div class="slide">

      <img src="IMG-20260725-WA0015.jpg" alt="Foto kita">

      <h2>Aku Menyesal</h2>

      <p>
        Aku menyesal sudah membuat kamu kecewa,
        sedih, atau bahkan terluka karena sikapku.
      </p>

      <p>
        Aku berharap kamu tahu kalau aku benar-benar menyesal.
      </p>

    </div>


    <!-- SLIDE 3 -->

    <div class="slide">

      <img src="IMG-20260709-WA0001.jpg" alt="Foto kita">

      <h2>Terima Kasih❤️</h2>

      <p>
        Terima kasih sudah pernah sabar menghadapi aku.
        Terima kasih untuk semua waktu,
        perhatian, dan kebaikan yang kamu kasih.
      </p>

    </div>


    <!-- SLIDE 4 -->

    <div class="slide">

      <img src="IMG-20260524-WA0079.jpg" alt="Foto kita">

      <h2>Aku Akan Berusaha🌷</h2>

      <p>
        Aku nggak mau permintaan maaf ini
        cuma menjadi kata-kata.
      </p>

      <p>
        Aku ingin belajar dari kesalahanku
        dan berusaha menjadi seseorang yang lebih baik.
      </p>

    </div>


    <!-- SLIDE 5 -->

    <div class="slide">

      <img src="IMG-20260826-WA0010.jpg" alt="Foto kita">

      <div class="big-heart">❤️</div>

      <h2>Maafin Aku Ya...</h2>

      <p>
        Aku tahu mungkin kata maaf
        nggak bisa langsung memperbaiki semuanya.
      </p>

      <p>
        Tapi kalau kamu masih mau,
        aku ingin memperbaiki semuanya pelan-pelan.
      </p>

      <p>
        <b>Maukah kamu memaafkanku?</b>
      </p>

      <button onclick="forgive()">
        IYA, AKU MAAFIN❤️
      </button>

      <div id="thanks">
        <h2>Terima kasih❤️</h2>
        <p>
          Kamu nggak tahu betapa berartinya
          jawaban itu buat aku
        </p>
        <p>
           Aku janji akan lebih menghargai kamu. 
        </p>
        <div class="big-heart">💕</div>
      </div>

    </div>


    <!-- NAVIGASI -->

    <div class="buttons">

      <button onclick="prevSlide()">
        ←
      </button>

      <button onclick="nextSlide()">
        →
      </button>

    </div>


    <!-- DOT -->

    <div class="dots">

      <span class="dot active"></span>
      <span class="dot"></span>
      <span class="dot"></span>
      <span class="dot"></span>
      <span class="dot"></span>

    </div>

  </div>


  <script>

    /* =====================
       PASSWORD
      ====================== */   

    fungsi checkPassword() {

      konstanta password  =
        document.getElementById("password").value;

      jika (password === "0922") {

        document.getElementById("login").style.display = "none";

        document.getElementById("content").style.display = "block";

        // Coba mulai musik
        document.getElementById("music").play().catch(() => {});

      } lain {

        document.getElementById("error").style.display = "block";

      }
    }


    /* =====================
       SLIDE
     ====================== */  

    biarkan currentSlide  =  0;

    konstanta slides  =
      document.querySelectorAll(".slide");

    konstanta dots  =
 dokumen. querySelectorSemua(".dot");querySelectorSemua(".dot");


 fungsi Jika (arusSlide < 0) { jika (arusSlide0) {

 slide. 
 slide.  
      });;

 titik-titik. 
 dot.  dot.  
       });; });;

 slide 

 titik 

     } }


 fungsi 

 arusSlide ++; 

 Jika (currentSlide >= slide.panjang) { jika (currentSlide >= slide.panjang) {
 arusSlide = 
        }  } 

 showSlide (arusSlide);  showSlide (arusSlide);  

     } 


 fungsi 

/html>html>prevSlide(</

 Jika (arusSlide < 0) { 
 currentSlide = slide. 
        } } } 

      }  showSlide (arusSlide) 

     } 


      showSlideshowSlide(arusSlide) showSlideshowSlide(arusSlide
     } 
/* ===================== /* =====================

}

(

showSlideshowSlide


     /* ===================== 
/* =====================
}

 dokumen 
       . 
        .  

        jika (event.kunci   ===   "Masuk") {
          checkPassword();
        }

      });


              ====================== *    
        ====================== *    
 /* ===================== /    

 /   

)

}

}

            ====================== */ 
 Math.random() * 100 + "vw"; 

       heart.style.fontSize = 
 (Math.random() * 15 + 12) + "px"; 

       heart.style.animationDuration = 
 (Math.random() * 3 + 4) + "s"; 

           setTimeout(() => {  setTimeout(() => {    

           setTimeout(() => {     
 /* =====================     
 setInterval (createHeart, 500); 

            ====================== */          /* =====================           /* =====================          

   /* =====================       

  </script>

</
</


