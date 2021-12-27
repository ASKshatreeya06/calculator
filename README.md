# calculator
#include<stdio.h>
#include<stdlib.h>
#include<conio.h>
main(){
	int a;
    printf("(1) this is for addintion \n");
    printf("(2) this is for substraction\n");
    printf("(3) this is for multiplication\n");
    printf("(4) this is for division\n");
    printf("(5) this is for finding number even or odd\n\t");
    scanf("%d",&a);
    switch(a){
    	case 1:
    		add();
    		break;
    		case 2:
    			sub();
    			break;
    			case 3:
    				mul();
    				break;
    				case 4:
    					divide();
    					break;
    					case 5:
    						evodd();
    						break;
    						default:
    							printf(" please enter vailide number");
    				
	}
	printf("\n\t press 0 go back to mune");
	printf("\n\t press any number for exit\n\t");
	int b;
	scanf("%d",&b);
	if(b==0){
		main();
	}
	else{
		exit(0);
	}
	
	return 0;
}
evodd(){
	int a;
	printf("enter the a number : \n");
	scanf("%d",&a);
	if(a%2==0){
		printf("this nmber is even");
		
	}
	else{
		printf("this number is odd");
		}
}
add(){
    int a,b;
    printf("enter two number for addition: \n");
    scanf("\t%d\n\t%d",&a,&b);
    printf("sum of two number: %d",a+b);
}
mul(){
    float a,b;
    printf("enter two number for multiplication :\n ");
    scanf("\t%f\n\t%f",&a,&b);
    printf(" multiple of two number : %f",a*b);
}
sub(){
    float a,b;
    printf("enter two number for substraction\n");
    scanf("\t%f\n\t%f",&a,&b);
    printf("substract two number : %f",a-b);
}
divide(){
    float a,b;
    printf("enter two number for divide\n");
    scanf("\t%f\n\t%f",&a,&b);
    printf("divide of two number : %f",a/b);
}
