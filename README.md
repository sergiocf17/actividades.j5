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
