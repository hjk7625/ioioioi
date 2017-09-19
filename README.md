# 공

float x = 100; 
float y = 0;

float speed = 0;
float gravity = 0.1;

void setup() {
  size(300, 600);
}

void draw() {
  background(255);
  
  fill(0);
  noStroke();
  ellipse(width/2, y, 20, 20);

 y = y + speed;
speed = speed + gravity;

if(y > height) {
  speed =  speed * - 0.95;
  y= height;
}
}
  
