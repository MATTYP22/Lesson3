# Lesson3

int l_motor=0;
int r_motor=2;
int speed=50;
int top_hat=3;
int on_line=200;
int off_line=800;
int f_target=1000;
int slow = 15;
int target_fronts=1500;


//FUNCTIONS DEFINTIONS

int forward(){
  motor(l_motor,speed);
  motor(r_motor,speed);
 }
 int l_turn(){
  motor(l_motor,slow);
  motor(r_motor,speed);

}
int r_turn(){
  motor(l_motor,speed);
  motor(r_motor,slow);
}
in line_follow(){  
  while (analog(f_target) < on_line) {
  
	if (analog(top_hat) < on_line) {
    	 //Not on line, turning left //
     l_turn();
      }




int main()

{//find line//
  while (analog(top_hat) <= off_line) {
	forward();
 	while(analog(f_target)<=target_fronts){
	
  }
  }
  ao();
   line_follow();


	printf("Hello, World!\n");
	return 0;
}
