let bgColor;
let textColor;

function setup() {
  createCanvas(900, 800);
  randomizeColors();
}

function draw() {
  background(bgColor);
  fill(textColor);
  textSize(64);
  textAlign(CENTER, CENTER);
 
  let maximo = width;
  let minimo = 0;
  let palavra = "José Siqueira Rosas";
  let quantidade = map(mouseX, 0, width, 1, palavra.length);
  let parcial = palavra.substring(0, quantidade);
  text(parcial, 400, 400);
}

function mouseClicked() {
  randomizeColors();
}

function randomizeColors() {
  bgColor = color(random(255), random(255), random(255));
  textColor = color(random(255), random(255), random(255));
}
