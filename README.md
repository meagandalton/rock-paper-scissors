# rock-paper-scissors
p1Selects();
var player1="";
var player2="";

function p1Selects(){
  var play = true;
  while (play===true){
    var p1=prompt("Player 1, do you want rock, paper, or scissors? ")
    if (p1==="rock"|| p1==="paper" || p1==="scissors"){
      player1=p1;
      p2Selects();
      play=false;
    }else{
      alert("Please select rock, paper, or scissors.");
      play=true;
    }
  }
}

function p2Selects(){
  var play = true;
  while (play===true){
    var p2=prompt("Player 2, do you want rock, paper, or scissors? ")
    if (p2==="rock"|| p2==="paper" || p2==="scissors"){
      player2=p2;
      game();
      play=false;
    }else{
      alert("Please select rock, paper, or scissors.");
      play=true;
    }
  }
}

function game(){
  if (player1===player2){
    alert("It is a tie!");
  } else if (player1==="rock" && player2==="scissors"){
    alert("Player 1 wins!");
  } else if (player1==="scissors" && player2==="paper"){
    alert("Player 1 wins!");
  } else if (player1==="paper" && player2==="rock"){
    alert("Player 1 wins!");
  }else{
    alert("Player 2 wins!");
  } 
}
