Static Block

package StaticBlock;

public class Initializer {
   static int initialvalue;
   static{
       initialvalue= 1000;
       System.out.println("Static Block: " +initialvalue);
   }
}
public class Main {
    public static void main(String[]args)
    {
     System.out.println("Before instance: " +Initializer.initialvalue);
     Initializer i= new Initializer();
     System.out.println("After instance: " +Initializer.initialvalue);
    }
}
