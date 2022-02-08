function setup() {
  createCanvas(windowWidth, windowHeight);
  noStroke();
  for (let i = 0; i < 1000; i++) {
    fill(random(255), random(255), random(255), random(255));
    ellipse(random(windowWidth), random(windowHeight), random(100)); 
  }
}
