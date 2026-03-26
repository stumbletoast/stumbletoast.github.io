---
layout: null
---

<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>

body{
  margin:0;
  background:#ffffff;
  font-family:sans-serif;
}

/* タイトル */

#title{
  text-align:center;
  margin-top:60px;
  font-size:1.5em;
  letter-spacing:0.2em;
}

/* ボタンエリア */

.buttonRow{
  margin-top:100px;
  display:flex;
  justify-content:center;
  align-items: flex-start;
}

/* ボタン */

#nextButton{
  width:400px;
  cursor:pointer;

  transform: translate(-400px, -200px);
}

/* --- 修正箇所：#thirdButton のみ --- */

#thirdButton {
  width: 50px;  /* 横幅はあなたの指定通り */
  height: auto; /* ★【重要】これを追加して比率を保つ */
  cursor: pointer;

  /* ★【重要】ここを自由に変更して位置を調整してください */
  /* translate(横方向の移動, 縦方向の移動) */
  /* 例: 右に50px、下に100px移動したい場合 -> translate(50px, 100px) */
  /* 例: 左に20px、上に30px移動したい場合 -> translate(-20px, -30px) */
  transform: translate(0px, 0px); 
}

#fourthButton {
  width: 100px;  /* 横幅はあなたの指定通り */
  height: auto; /* ★【重要】これを追加して比率を保つ */
  cursor: pointer;

  /* ★【重要】ここを自由に変更して位置を調整してください */
  /* translate(横方向の移動, 縦方向の移動) */
  /* 例: 右に50px、下に100px移動したい場合 -> translate(50px, 100px) */
  /* 例: 左に20px、上に30px移動したい場合 -> translate(-20px, -30px) */
  transform: translate(-500px, 400px); 
}

#fifthButton {
  width: 200px;  /* 横幅はあなたの指定通り */
  height: auto; /* ★【重要】これを追加して比率を保つ */
  cursor: pointer;

  /* ★【重要】ここを自由に変更して位置を調整してください */
  /* translate(横方向の移動, 縦方向の移動) */
  /* 例: 右に50px、下に100px移動したい場合 -> translate(50px, 100px) */
  /* 例: 左に20px、上に30px移動したい場合 -> translate(-20px, -30px) */
  transform: translate(50px, 600px); 
}


/* スマホ用の設定もそのまま維持 */
/* スマホ用の設定（ここを入れ替え） */
@media (max-width:600px) {

  #nextButton {
    width: 70vw;
    max-width: 250px;
    transform: translate(0, 0);
  }

  #thirdButton {
    width: 8vw; /* サイズ：ここを好きな数字に変えられます */
    max-width: 80px;
    transform: translate(0px, 0px); /* 位置：ここを好きな数字に変えられます */
  }

  #fourthButton {
    width: 15vw; /* サイズ：ここを好きな数字に変えられます */
    max-width: 150px;
    transform: translate(-20px, 500px); /* 位置：ここを好きな数字に変えられます */
  }

  #fifthButton {
    width: 20vw; /* サイズ：ここを好きな数字に変えられます */
    max-width: 150px;
    transform: translate(-50px, 400px); /* 位置：ここを好きな数字に変えられます */
  }

} /* ← 最後に一回だけ閉じる */


</style>
</head>

<body>

<h1 id="title">STUMBLETOAST!!</h1>

<div class="buttonRow">

<img id="nextButton" src="assets/1B.png">

<img id="thirdButton" src="assets/2B.png">

<img id="fourthButton" src="assets/3B.png">

<img id="fifthButton" src="assets/4B.png">


</div>

<script>

document.getElementById("nextButton").onclick=()=>{
  location.href="next.html"
}

document.getElementById("thirdButton").onclick=()=>{
  location.href="third.html"
}

document.getElementById("fourthButton").onclick=()=>{
  location.href="fourth.html"
}

</script>

</body>
</html>