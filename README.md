# Snek
snake but bad

class Snake {
constructor() {
this.totalMoves_ = 0;
}
move(squaresMoved) {
if (squaresMoved > 0) return this.totalMoves_ = this.totalMoves_ + squaresMoved + " squares foward" 
else return this.totalMoves_ = this.totalMoves_ + squaresMoved + " squares backwards"
}
turn(snakeDirection) {
if (snakeDirection > 0) return this.totalMoves_ = this.totalMoves_ + snakeDirection + " squares backwards"
else return this.totalMoves_ = this.totalMoves_ + snakeDirection + " squares foward"
}
get squaresMoved() {
return this.totalMoves_;
}
}

let snake1 = new Snake();
let snake2 = new Snake();
let snake3 = new Snake();
let snake4 = new Snake();
snake1.move(-5);
snake2.move(10);
console.log("snake1 moved: ", snake1.squaresMoved);
console.log("snake2 moved: ", snake2.squaresMoved);
snake3.turn(8);
snake4.turn(-12);
console.log("snake3 turned: ", snake3.totalMoves_);
console.log("snake4 turned: ", snake4.totalMoves_);
