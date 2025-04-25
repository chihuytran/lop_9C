<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>Lớp 9C</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background: #f0f8ff;
      overflow-x: hidden;
      transition: background 1s ease;
    }

    #introText {
      text-align: center;
      font-size: 48px;
      margin-top: 100px;
      opacity: 0;
      transition: opacity 1s ease;
      color: #333;
      position: relative;
      z-index: 2;
    }

    #mainImage {
      display: none; /* Ẩn mặc định */
      margin: 40px auto;
      width: 250px;
      opacity: 0;
      transition: opacity 1s ease;
      filter: drop-shadow(0 0 20px rgba(0,0,0,0.2));
      position: relative;
      z-index: 2;
    }

    .fog {
      position: absolute;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background: #ffffffbb;
      background-size: cover;
      opacity: 0.3;
      z-index: 1;
      pointer-events: none;
    }

    #container {
      display: none;
      padding: 80px 20px;
      background-color: #d6f5f7;
      min-height: 100vh;
      position: relative;
    }

    #frame {
      background:#ffffffbb;
      max-width: 1000px;
      margin: 0 auto;
      border: 2px solid #aaa;
      padding: 20px;
      border-radius: 12px;
      background-color: c
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      position: relative;
      z-index: 2;
    }

    #frame h2 {
      text-align: center;
      font-size: 36px;
      margin-bottom: 30px;
    }

    .buttons {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
    }

    .btn3d {
      padding: 15px 25px;
      font-size: 16px;
      font-weight: bold;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: all 0.2s ease;
      box-shadow: 0 6px #999;
      min-width: 100px;
    }

    .btn3d:active {
      box-shadow: 0 3px #666;
      transform: translateY(3px);
    }

    .blue {
      background-color: #4da6ff;
      color: white;
    }

    .pink {
      background-color: #ff80bf;
      color: white;
    }

    #classInfoBtn {
      position: fixed;
      top: 20px;
      left: 20px;
      z-index: 3;
      background-color: #f9a825;
      color: white;
    }

    #sideImages {
      position: fixed;
      top: 0;
      width: 100%;
      pointer-events: none;
      z-index: 1;
    }

    .side-img {
      width: 120px;
      opacity: 0.85;
      position: absolute;
      transition: transform 0.3s ease;
    }

    .side-img.left {
      left: 0;
      transform: rotate(-25deg);
    }

    .side-img.right {
      right: 0;
      transform: rotate(-10deg);
    }
     .side-img.left1 {
      left: 0;
      transform: rotate(20deg);
    }

    .side-img.right1 {
      right: 0;
      transform: rotate(15deg);
    }

    #classInfo {
      display: none;
      text-align: center;
      font-size: 24px;
      padding: 40px;
      color: #333;
      z-index: 4;
      background-color: #ffffffcc;
    }
     #albumBtn {
  position: fixed;
  top: 20px;
  right: 20px;
  z-index: 3;
  background-color: #e91e63;
  color: white;
}

  </style>
</head>
<body>

  <div id="introText">Chào mừng bạn đến với lớp 9C</div>
  <img id="mainImage" src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/ChatGPT_logo.svg/2048px-ChatGPT_logo.svg.png" alt="Ảnh chính">

  <div class="fog"></div>

  <button class="btn3d" id="classInfoBtn">Thông tin của lớp</button>
  <button class="btn3d" id="albumBtn">Ghi album</button>

  <div id="classInfo">Hiện tại không có thông tin gì</div>

  <div id="sideImages">
    <img src="Picture1.jpg" class="side-img left" style="top: 200px; left: 30px;">
    <img src="Picture2.jpg" class="side-img left1" style="top: 400px; left: 40px;">
    <img src="Picture3.jpg" class="side-img right" style="top: 260px; right: 30px;">
    <img src="Picture4.jpg" class="side-img right1" style="top: 450px; right: 40px;">
  </div>

  <div id="container">
    <div id="frame">
      <h2>LỚP 9C Ở ĐÂY</h2>
      <div class="buttons" id="buttonContainer"></div>
    </div>
  </div>

  <script>
    const intro = document.getElementById('introText');
    const image = document.getElementById('mainImage');
    const container = document.getElementById('container');
    const body = document.body;
    const classInfoBtn = document.getElementById('classInfoBtn');
    const classInfo = document.getElementById('classInfo');
    const buttonContainer = document.getElementById('buttonContainer');
    const albumBtn = document.getElementById('albumBtn');
    albumBtn.onclick = () => {
    window.open("https://online.fliphtml5.com/phxda/cxvj/"); // Thay bằng link thật của bạn
   };

    const texts = [
      "Chào mừng bạn đến với lớp 9C",
      "Trang web này dành riêng cho lớp 9C-THCS Nam Hồng",
      "Được phát triển và hoàn thiện bởi Trần Chí Huy",
      "Cùng với sự trợ giúp của"
    ];

    function showTexts(index = 0) {
      if (index >= texts.length) {
        setTimeout(() => {
          // Sau khi kết thúc intro, hiện ảnh lớp
          image.style.display = "block";
          setTimeout(() => {
            image.style.opacity = 1;
          }, 100);
        }, 500);

        setTimeout(() => {
          intro.style.opacity = 0;
          image.style.opacity = 0;
        }, 2500);

        setTimeout(() => {
          document.querySelector('.fog').style.display = 'none';
          body.style.background = "#d6f5f7";
          container.style.display = "block";
        }, 3500);
        return;
      }

      intro.textContent = texts[index];
      intro.style.opacity = 1;

      setTimeout(() => {
        intro.style.opacity = 0;
        setTimeout(() => {
          showTexts(index + 1);
        }, 1000);
      }, 1000);
    }

    window.onload = () => {
      showTexts();
    };

    const namesAndLinks = [
      { name: "Việt An", color: "blue", url: "https://www.facebook.com/yuean1046" },
      { name: "Hà An", color: "pink", url: "https://www.facebook.com/han.nguyen.12092" },
      { name: "Việt Anh", color: "pink", url: "https://www.facebook.com/viet.anh309" },
      { name: "Phương Anh", color: "pink", url: "https://www.facebook.com/profile.php?id=100075183654953" },
      { name: "Lê Bùi Gia Bảo", color: "blue", url: "https://www.facebook.com/profile.php?id=100081807525502" },
      { name: "Nguyễn Hữu Gia Bảo", color: "blue", url: "https://example.com/2" },
      { name: "Nguyễn Gia Bảo", color: "blue", url: "https://www.facebook.com/profile.php?id=61572557385653" },
      { name: "Ánh Dương", color: "pink", url: "https://example.com/4" },
      { name: "Minh Hiếu", color: "blue", url: "https://www.facebook.com/profile.php?id=100077097866531" },
      { name: "Nhật Huy", color: "blue", url: "https://www.facebook.com/nhat.huy.921244" },
      { name: "Chí Huy", color: "blue", url: "https://www.facebook.com/tran.huy.348157/" },
      { name: "Văn Hùng", color: "blue", url: "https://www.facebook.com/hung18t7" },
      { name: "Phương Linh", color: "pink", url: "https://www.facebook.com/phuong.linh.671494" },
      { name: "Khánh Linh", color: "pink", url: "https://www.facebook.com/khanh.linh.649107" },
      { name: "Tuệ Linh", color: "pink", url: "https://www.facebook.com/le.tue.linh.303694" },
      { name: "Thảo Linh", color: "pink", url: "https://www.facebook.com/thaolinh.p0" },
      { name: "Thanh Thảo", color: "pink", url: "https://www.facebook.com/thanh.thao.lknhanhoots" },
      { name: "Minh Thành", color: "blue", url: "https://www.facebook.com/profile.php?id=100091975759674" },
      { name: "Đức Thiện", color: "blue", url: "https://www.facebook.com/profile.php?id=100072824761992" },
      { name: "Mạnh Thắng", color: "blue", url: "https://www.facebook.com/profile.php?id=61559974231259" },
      { name: "Hoàng Anh Tuấn", color: "blue", url: "https://www.facebook.com/tuan.hoang.358576" },
      { name: "Nguyễn Minh Tuấn", color: "blue", url: "https://www.facebook.com/nguyen.minh.tuan.301487" },
      { name: "Phan Anh Tuấn", color: "blue", url: "https://www.facebook.com/profile.php?id=61558831420915" },
      { name: "Linh Nhy", color: "pink", url: "https://www.facebook.com/n.nhy15" },
      { name: "Thiên Nam", color: "blue", url: "https://www.facebook.com/paul.s.disciphes.tran" },
      { name: "Kỷ Nguyên", color: "blue", url: "https://www.facebook.com/profile.php?id=61570788825358" },
      { name: "Huyền Trân", color: "pink", url: "https://www.facebook.com/htran2101" },
      { name: "Tường Vy", color: "pink", url: "https://www.facebook.com/profile.php?id=100080126114417" },
      { name: "Nam Phong", color: "blue", url: "https://www.facebook.com/profile.php?id=61557038235107" },
      { name: "Bảo Ngọc", color: "pink", url: "https://www.facebook.com/mzgc.paii" },
      { name: "Thành An", color: "blue", url: "https://www.facebook.com/profile.php?id=61551468487445" },
      { name: "Minh Phương", color: "pink", url: "https://www.facebook.com/minh.phuong.637828" },
      { name: "Hoài Thu", color: "pink", url: "https://www.facebook.com/profile.php?id=100078925185328" },
      { name: "Thanh Tâm", color: "pink", url: "https://www.facebook.com/profile.php?id=100045739153687" },
      { name: "Gia Nhi", color: "pink", url: "https://www.facebook.com/nhii.nguyen.929894" },
      { name: "Anh Quân", color: "blue", url: "https://www.facebook.com/profile.php?id=61554936463697" },
      { name: "Thầy giáo chủ nhiệm: Kiều Mạnh Hoàng", color: "blue", url: "https://www.facebook.com/profile.php?id=100008250704964" }
      // thêm đủ 36 người tại đây
    ];

    namesAndLinks.forEach(item => {
      const btn = document.createElement("button");
      btn.textContent = item.name;
      btn.className = `btn3d ${item.color}`;
      btn.onclick = () => window.open(item.url, "_blank");
      buttonContainer.appendChild(btn);
    });

    let showingInfo = false;
    classInfoBtn.onclick = () => {
      showingInfo = !showingInfo;
      if (showingInfo) {
        container.style.display = "none";
        classInfo.style.display = "block";
      } else {
        container.style.display = "block";
        classInfo.style.display = "none";
      }
    };
  </script>
</body>
</html>
