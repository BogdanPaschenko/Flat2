package Homework;
import java.util.Scanner;
public class Flat {

	public static void main(String[] args) {
		Scanner sc = new Scanner (System.in);
	System.out.println("Enter flat number");
	int flat = sc.nextInt();
	if ((flat>=1)&&(flat<=144)){
	int podezd = (flat+(36-1))/36;
	int floornumber= (flat-(podezd-1)*36-1)/4+1;
	
	System.out.println ("Квартира находится в " + podezd + " подъезде, на "+floornumber+" этаже");	
	}
	else{
		System.out.println("Такой квартиры в этом доме не существует :(");
	}
	sc.close();

	}

}
