let x = 320;
let y = 180;
let xx = 200;
let yy = 110;
let xxx = 380;
let yyy = 90;
let xxxx = 380;
let yyyy = 90;
let xxxxx = 380;
let yyyyy = 90;
let xspeed = -8;
let yspeed = 3;
let xxspeed = 5;
let yyspeed = 2;
let xxxspeed = -4;
let yyyspeed = 3;
let xxxxspeed = -10;
let yyyyspeed = 1;
let xxxxxspeed = 2;
let yyyyyspeed = -7;

let r = 38;

function setup() {
  createCanvas(640, 360);
}

function draw() {
  // for (let i = 0; i < 2; i++) { fill(random(255), random(255), random(255), random(255)); ellipse(random(windowWidth), random(windowHeight), random(100)); } 
  
  background(255);
  ellipse(x, y, r*2, r*2);
  fill (random(255),random(255),random(255))
  x += xspeed;
  y += yspeed;
  if (x > width - r || x < r) {
    xspeed = -xspeed;
  }
  if (y > height - r || y < r) {
    yspeed = -yspeed;
  }
  
  //Ball 2
  ellipse(xx, yy, r*2, r*2);
  fill (random(255),random(255),random(255))
  xx += xxspeed;
  yy += yyspeed;

  if (xx > width - r || xx < r) {
    xxspeed = -xxspeed;
  }
  if (yy > height - r || yy < r) {
    yyspeed = -yyspeed;
  }

  //Ball 3
  ellipse(xxx, yyy, r*2, r*2);
  fill (random(255),random(255),random(255))
  xxx += xxxspeed;
  yyy += yyyspeed;
  if (xxx > width - r || xxx < r) {
    xxxspeed = -xxxspeed;
  }
  if (yyy > height - r || yyy < r) {
    yyyspeed = -yyyspeed;
  }
  
  //Ball 4
  
  ellipse(xxxx, yyyy, r*2, r*2);
  fill (random(255),random(255),random(255))
  xxxx += xxxxspeed;
  yyyy += yyyyspeed;
  if (xxxx > width - r || xxxx < r) {
    xxxxspeed = -xxxxspeed;
  }
  if (yyyy > height - r || yyyy < r) {
    yyyyspeed = -yyyyspeed;
  }
  
  //Ball 5
  ellipse(xxxxx, yyyyy, r*2, r*2);
  fill (random(255),random(255),random(255))
  xxxxx += xxxxxspeed;
  yyyyy += yyyyyspeed;
  if (xxxxx > width - r || xxxxx < r) {
    xxxxxspeed = -xxxxxspeed;
  }
  if (yyyyy > height - r || yyyyy < r) {
    yyyyyspeed = -yyyyyspeed;
  }
}
