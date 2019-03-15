# actividades.j5
las actividades de clase Enero2019
Sergio Cardenas Flores 1545550 N5

Act.1

function setup() {
  createCanvas(800, 800);
}

function draw() {
  background(0);
	line(800,800,399,399);
	line(00,800,399,399);
	line(399,399,399,0)
	fill(152);
	stroke(255);
}


Act.2

function setup() {
  createCanvas(300, 300);
}

function draw() {
  background(220);
	rect(0,0,100, 299);
	fill(0,0,200);
	rect(100,0,100, 299);
	fill(200,0,0);
	rect(200,0,99, 299);
	fill(0,200,0);
}



ACTIVIDAD DEL DIA 8 DE FEBRERO 

var num;
function setup() {
  createCanvas(400, 400);
}

function draw() {
  	num =int(random(1, 7));
	if(mouseIsPressed){
		if(num==1){
			uno();
		}
		if(num==2){
			dos();
		}
		if(num==3){
			tres();
		}
		if(num==4){
			cuatro();
		}
		if(num==5){
			cinco();
		}
		if(num==6){
			seis();
		}
	
}
}
	
function uno(){
	background(220);
	strokeWeight(20);
	rect(100,100,200,200);
	ellipse (200, 200, 10, 10);
	
}

function dos(){
	background(220);
	strokeWeight(20);
	rect(100,100,200,200);
	ellipse (150, 150, 10, 10);
	ellipse (250, 250, 10, 10);
}

function tres(){
	background(220);
	strokeWeight(20);
	rect(100,100,200,200);
	ellipse (150, 150, 10, 10);
	ellipse (250, 250, 10, 10);
	ellipse (200, 200, 10, 10);
}

function cuatro(){
	background(220);
	strokeWeight(20);
	rect(100,100,200,200);
	ellipse (150, 150, 10, 10);
	ellipse (150, 250, 10, 10);
	ellipse (250, 250, 10, 10);
	ellipse (250, 150, 10, 10);

}


15 de febrero

var pelotas =[];
function setup() {
  createCanvas(600, 600);
	for (var i=0; i <100;i++){
    pelotas[i] = new Pelota();
  }
}

function draw() {
  background(220);
  for (var i = 0; i < 50; i++){
    pelotas[i].mostrar();
    pelotas[i].mover();
    
    if (pelotas[i].salirx()){
      pelotas[i].rebotarx();
    }
  
    if (pelotas[i].saliry()){
      pelotas[i].rebotary();
}
  }
}

22 de febrero 

class Pelota {
	constructor() {
		this.x1 = 20;
		this.y1 = 20;
		this.velx = random(3,10);
		this.vely = random(3,10);
		this.posx = random(0, 400);
		this.posy = random(0, 400);
		this.R = random(0, 255);
		this.G = random(0, 255);
		this.B = random(0, 255);
	}

	mostrar() {
		ellipse(this.posx, this.posy, this.x1, this.y1);
		fill(this.R, this.G, this.B);
	}
	mover() {
		this.posx = this.posx + this.velx
		this.posy = this.posy + this.vely;

	}
	salir() {
		var res;
		if (this.posx < 0 || this.posx > width || this.posy < 0 || this.posy > height ) {
			res = true
		} else {
			res = false
		}
		return res;
	}
	rebotar() {
		this.velx = -this.velx
		this.vely = -this.vely
	}
}
