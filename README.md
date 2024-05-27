Boas vindas ao meu perfil 💙💙
Meu nome é Ana Beatriz Freitas

Estou estudando na Alura
Estou me desenvolvendo na linguagem JavaScript
Utilizo esse espaço para minha organização e compartilhamento dos meu projetos desenvolvidos
Você pode entrar em contato comigo 📫
00001128113697sp@al.educacao.sp.gov.br

@anabiaoliveirafabricio@gmail.com

![]([link](https://tenor.com/pt-BR/view/isso-foi-fofo-gif-2514319886472714943))

projeto 1
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
} function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
}let cor;
let circuloX; // horizontal
let circuloY; // vertical

function setup() {
  createCanvas(400, 400);
  background(color(100, 0 , 0));
  cor = color(random(0, 255), random(0, 255), random(0, 255));
  
  circuloX = [0, 0, 0];
  circuloY = [random(height), random(height), random(height)];
}

function draw() {
  
  fill(cor);
  
  for(let contador in circuloX) {
    circle(circuloX[contador], circuloY[contador], 50);    
    circuloX[contador]+= random(0,3);
    circuloY[contador]+= random(-3,3); 
    
    if(circuloX[contador] >= width){
      circuloX[contador] = 0;
      circuloY[contador] = random(height);
    }
  }
  
  if(mouseIsPressed){
    cor = color(random(0, 255), random(0, 255), random(0, 255), random(0, 100));
  }
}

projeto 2 
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
}function setup() {
  createCanvas(400, 400);
}

function draw() {
  background("white");
  fill("black");
  textSize(64);
  textAlign(CENTER, CENTER)
  
  let maximo = width;
  let minimo = 0;
  let palavra = "ana beatriz";
  let quantidade = map(mouseX, 0, width, 1, palavra.length);
  let parcial = palavra.substring(0,quantidade);
  text(parcial,200,200);
  
//  if(mouseX < 50){
//    let palavra = "C";
//    text(palavra, 200, 200);
//  } else {
//    let palavra = "Caminhante";
//    text(palavra, 200, 200);
//  }
} let campoNome;

if (campoNome === undefined) {
    console.log("O campo NOME está vazio!");
} function setup() {
  createCanvas(400, 400);
}

function inicializaCores(){
  background("white");
  fill("black");
  textSize(64);
  textAlign(CENTER,CENTER);
}

function draw() {
  inicializaCores();
  
  let maximo = width;
  let minimo = 1;
  //mouseX, 0, width ==> 0, palavra.length
  let palavra = "ana bia";
  let quantidade = map(mouseX, 0, width, 1, palavra.length);
  //console.log(quantidade);
  let parcial = palavra.substring(0,quantidade);
  text(parcial,200,200);
}
