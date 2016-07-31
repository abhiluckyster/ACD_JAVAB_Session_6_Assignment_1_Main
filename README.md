# ACD_JAVAB_Session_6_Assignment_1_Main

package AbstractAndInterface;
public interface Interface2Methods {
	public abstract void method(int num);
	}
	
package AbstractAndInterface;
public class PrintInterfaceClass implements Interface2Methods {
	public void method(int num) {
		System.out.println("Printing the number for the first class : "+num);
	}
}

package AbstractAndInterface;
public class PrintInterfaceSquareClass implements Interface2Methods{
	public void method(int num) {
		System.out.println("Printing the square of the number for the second class : "+(num*num));
	}
}

package AbstractAndInterface;
import java.util.Scanner;
public class InterfaceTwoClasses {
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		System.out.println("Enter the number");
		int num = scanner.nextInt();
		PrintInterfaceClass pic = new PrintInterfaceClass();
		PrintInterfaceSquareClass pisc = new PrintInterfaceSquareClass();
		pic.method(num);
		pisc.method(num);
		scanner.close();
	}
}


