## twitter018 | #つぶやきProcessing 
https://twitter.com/nicolasbaez/status/1399562826843295744?s=20

![twitter](https://github.com/nicolasbaez/twitter018/blob/main/twitter018.gif)
```processing
void setup() {
  size(500, 500, P3D);
}
float i, k, w=500;
void draw() {
  clear();
  noFill();
  for (i=0; i<w; i+=9) {
    stroke(#9933CC, noise(i, k)*w);
    push();
    translate(i, map(sin(radians(i+k)), 0, 1, 0, noise(i)*w));
    sphereDetail(1);
    rotateX(k/(5*PI));
    sphere(map(sin(i), 0, 1, 9, 64));
    pop();
  }
  k++;
}
```
