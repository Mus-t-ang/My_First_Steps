# My_First_Steps
HTML, CSS, JS, Java

// Excersice 1
// Code to create a 250 X 250 image and change its color.
//var img = new SimpleImage (250, 250);
//for (var pixel of img.values()) {
//    pixel.setRed(0);
//    pixel.setGreen(15);
//    pixel.setBlue(0);
//}
//print (img);
// Excercise 2
// Code to change the color on each 1/3rd of the image.
var img = new SimpleImage ("smalluniverse.jpg");
var width = img.getWidth();
Math.round(width);
for (var pixel of img.values()) {
    var x = pixel.getX();
    if (x < width/3) {
        pixel.setRed(255);
    }
    else {
        if (x >= width/3 && x < width*2/3) {
            pixel.setGreen(255);
        }
        else {
            if (x >= width*2/3) {
                pixel.setBlue(255);
            }
} }
}
print (img);
