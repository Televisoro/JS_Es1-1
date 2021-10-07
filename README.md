<html>
  <head>
    <title>Es 1</title>
  </head>
    <body>
      <button onclick= "console.log('click da evento')">cliccami da evento</button>
      <button onclick ="funzioneClick('script')">cliccami script</button>
      <button id="btn3">cliccami da listener</button>

      <script>
        //Dichiarare una funzione e la richiamo allo stesso tempo
        // var funzioneClick = function(){
        //   console.log("click da script");
        // };

        var funzioneClick = function(stringa){
          console.log("click da "+ stringa);
        };
        
        //Prendo il bottne in una variabile
        var bottone3 = document.getElementById("btn3");
        bottone3.addEventListener("click", function(){
          funzioneClick("listener")
          bottone3.setAttribute("style","background-color: red");
        }
        );
      </script>
    </body>
</html>
