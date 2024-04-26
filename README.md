function setup() {
  createCanvas(800, 800);
}

function draw() {
  background("blue");
  fill("black");
  textSize(64);
  textAlign(CENTER,CENTER);
  
  let maximo = width;
  let minimo = 0;
  //mouseX, 0, width ==> 0, palavra.length
  let palavra = "José Siqueira Rosas";
  let quantidade = map(mouseX, 0, width, 1, palavra.length);
  //console.log(quantidade);
  let parcial = palavra.substring(0,quantidade);
  text(parcial,400,400);
  
  // if(mouseX <50) {
  // let palavra = "C";
  //text(palavra,200,200);
  //}else if (mouseX <100){
  //let palavra = "Ca";
  // text(palavra,200,200);
  //}else{
  //let palavra = "Estudante";
  // text (palavra,200,200);
  //}


  
}
