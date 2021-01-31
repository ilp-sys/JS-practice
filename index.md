<!DOCTYPE html>
<html lang ="ko">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>JavaScript Tutorial</title><!DOCTYPE html>
<html>
  <head>
    <title>Word Counter</title>
  </head>
  <body>
    <h1>Self-Introduction Document</h1>
            <!--event & event-handling-->>
    <textarea onkeydown='wordcounter();' class="form-control" rows="3" id="content">Please enter text.</textarea>
    <span id="count">(0/200)</span>
    <script>
      function wordcounter() 
      {
        //DOM
        var content = document.getElementById('content').value;
        if (content.length > 200)
        {
          content = content.sbstring(0,200);
<!DOCTYPE html>
<html lang ="ko">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>JavaScript Tutorial</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <h1>JavaScript Tutorial</h1>
    <script src="script.js"></script>
    <script>
        //insert text in html
        document.write('hello\n');
        //declare variabe and check data type
        var name = 'Jiwoo Ahn';
        var age = 20;
        //document.write(typeof name, "\n",  typeof age);
        document.write(name, "\n", age)
    </script>
    <ol>
      <li> <a href="random.html">Lotto number Drawer</a></li>
      <li> <a href="wordcount.html">Word Count</a></li>
      <li> <a href="ministar.html">Mini Star Carft</a></li>
    <ol>
  </body>
</html>
<!DOCTYPE html>
<html>
  <head>
      <title>Mini Star Craft</title>
      <style>
        .background{
          position: relative;
          background-image: url('background.png');
          background-size: 500px 330px;
          width: 500px;
          height: 330px;
        }
        #char{
          position: absolute;
          width: 100px;
          height: 100px;
          top: 100px;
          left: 60px;
          cursor: pointer;
        }
        #alien{
          position: absolute;
          width: 150px;
          height: 150px;
          top: 80px;
          right: 20px;
        }
        #attack{
          display: none;
          position: absolute;
          top: 140px;
          left: 150px;
          width: 50px;
          height: 30px;
          z-index: 2;
        }
      </style>
  </head>
  <body>
    <h1 id='hp'>HP: 5</h1>
    <div class='background'>
      <img id='char' src="char.png" alt="char">
      <img id='attack' src="attack.png" alt="attack">
      <img id='alien' src="alien.png" alt="alien">
    </div>
    <script 
    src="https://code.jquery.com/jquery-3.5.1.min.js"
    integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0="
    crossorigin="anonymous"></script>
    <script>
      //code.jquery.com
      //$(#id).val();
      var hp = 5;
      $('#char').click(function(){
        $('#attack').fadeIn();
        $('#attack').animate({left: '+300'});
        $('#attack').fadeOut(function(){
          //call back
          hp -= 1;
          $('#hp').text('HP: ' + hp);
          if(hp == 0){
            $('#alien').fadeOut();
          }
        });
        $('#attack').css({left:'150px'});
      });
    </script>
    <br></br>
    <a href="index.html">BACK TO HOME</a>
  </body>
</html>
<!DOCTYPE html>
<html>
  <head>
      <title>Lotto Number Drawer</title>
  </head>
  <body>
    <h1>Lotto Number Drawer</h1>
    <script>

      var lotto = [];
      while (lotto.length < 6) 
      {
        var num = parseInt(Math.random() * 45 + 1);
        if (lotto.indexOf(num) == -1) 
          lotto.push(num);
      }

      lotto.sort((a,b)=>a-b);

      var i;
      for(i = 0; i < 6; i++){
        document.write("<div>" + lotto[i] + "</div>");
      }
    </script>
    <a href="index.html">BACK TO HOME</a>
  </body>
</html>
<!DOCTYPE html>
<html>
  <head>
    <title>Word Counter</title>
  </head>
  <body>
    <h1>Self-Introduction Document</h1>
            <!--event & event-handling-->>
    <textarea onkeydown='wordcounter();' class="form-control" rows="3" id="content">Please enter text.</textarea>
    <span id="count">(0/200)</span>
    <script>
      function wordcounter() 
      {
        //DOM
        var content = document.getElementById('content').value;
        if (content.length > 200)
        {
          content = content.sbstring(0,200);
          document.getElementById('content').value = content;
        }
        document.getElementById('count').innerHTML = '(' + content.length + '/200)';
      }
      wordcounter();
    </script>
    <br></br>
    <a href="index.html">BACK TO HOME</a>
  </body>
</html>



          document.getElementById('content').value = content;
        }
        document.getElementById('count').innerHTML = '(' + content.length + '/200)';
      }
      wordcounter();
    </script>
    <br></br>
    <a href="index.html">BACK TO HOME</a>
  </body>
</html>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <h1>JavaScript Tutorial</h1>
    <script src="script.js"></script>
    <script>
        //insert text in html
        document.write('hello\n');
        //declare variabe and check data type
        var name = 'Jiwoo Ahn';
        var age = 20;
        //document.write(typeof name, "\n",  typeof age);
        document.write(name, "\n", age)
    </script>
    <ol>
      <li> <a href="random.html">Lotto number Drawer</a></li>
      <li> <a href="wordcount.html">Word Count</a></li>
      <li> <a href="ministar.html">Mini Star Carft</a></li>
    <ol>
  </body>
</html>
