<!DOCTYPE html>
<html lang="en">
  <head>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <div>
        <h1 class="header_text">Do you wanna go out with me?</h1>
      </div>
      <p>
        <a href="https://www.instagram.com/untoldcoding/">@untoldcoding</a>
      </p>
      <div class="gif_container">
        <img
          src="https://i.postimg.cc/pdNqPxx1/milk-and-mocha-cute.gif"
          alt="Cute animated illustration"
        />
      </div>
      <div class="buttons">
        <button class="btn" id="yesButton" onclick="nextPage()">Yes</button>
        <button
          class="btn"
          id="noButton"
          onmouseover="moveButton()"
          onclick="moveButton()"
        >
          No
        </button>

        <script>
          function nextPage() {
            window.location.href = "yes.html";
          }

          function moveButton() {
            var x =
              Math.random() *
              (window.innerWidth -
                document.getElementById("noButton").offsetWidth);
            var y =
              Math.random() *
              (window.innerHeight -
                document.getElementById("noButton").offsetHeight);
            document.getElementById("noButton").style.left = `${x}px`;
            document.getElementById("noButton").style.top = `${y}px`;
          }
        </script>
      </div>
    </div>
  </body>
</html>

body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;

  background: linear-gradient(rgb(0, 249, 236), rgb(71, 150, 229));
}

#noButton {
  position: absolute;
  margin-left: 150px;
  transition: 0.5s;
  margin-top: 30px;
}

#yesButton {
  position: absolute;
  margin-right: 150px;
  margin-top: 30px;
}

.header_text {
  font-family: "Nunito";
  font-size: 50px;
  font-weight: bold;

  text-align: center;
  margin-top: 20px;
  margin-bottom: 20px;
  color: #ffffff;
}

.text {
  font-family: "Nunito";
  font-size: 25px;
  font-weight: bold;
  color: white;
  text-align: center;
  margin-top: 20px;
  margin-bottom: 0px;
}

.buttons {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  margin-top: 20px;
  margin-left: 20px;
}

.btn {
  background-color: #017cff;
  color: white;
  font-weight: 600;
  padding: 15px 32px;
  text-align: center;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
  border: none;
  border-radius: 12px;
  transition: background-color 0.3s ease;
  box-shadow: 0 3px 3px black;
}

.btn:hover {
  background-color: #ffffff;
  color: #017cff;
}

.gif_container {
  display: flex;
  justify-content: center;
  align-items: center;
}
p {
  color: white;
  margin-left: 50%;
}
p a {
  color: rgb(255, 255, 255);
  font-size: 20px;
  font-weight: 600;
  opacity: 0.25;
}

<!DOCTYPE html>
<html lang="en">
  <head>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <div>
        <h1 class="header_text">Yeeyy ! Finally</h1>
      </div>
      <div class="gif_container">
        <img
          src="https://i.postimg.cc/wTDG30TB/yes.gif"
          alt="Cute animated illustration"
        />
      </div>
      <button class="btn" id="yesButton" onclick="nextPage()">
        Let's Fix a Date
      </button>
    </div>
  </body>
</html>

