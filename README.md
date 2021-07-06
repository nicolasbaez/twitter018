# twitter018
#つぶやきProcessing void setup(){size(500,500,P3D);}float i,k,w=500;void draw(){clear();noFill();for(i=0;i&lt;w;i+=9){stroke(#9933CC,noise(i,k)*w);push();translate(i,map(sin(radians(i+k)),0,1,0,noise(i)*w));sphereDetail(1);rotateX(k/(5*PI));sphere(map(sin(i),0,1,9,64));pop();}k++;}
