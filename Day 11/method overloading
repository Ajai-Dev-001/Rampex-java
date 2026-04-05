class Amazon{
    void delivery(){
        System.out.println("product will be delivered");
    }
}
class StandardDelivery extends Amazon {
    void delivery(){
        System.out.println("product will be delivered in 5 days");
    }
}
class ExpressDelivery extends Amazon {
    void delivery(){
        System.out.println("product will be delivered in 2 days");
    }
}
class PrimeDelivery extends Amazon {
    void delivery(){
        System.out.println("product will be delivered in 1 days");
    }
}
public class Main{
    public static void main(String[] arg){
        Amazon a;
        a=new Amazon();
        a.delivery();
         a=new StandardDelivery();
        a.delivery();
         a=new ExpressDelivery();
        a.delivery();
         a=new PrimeDelivery();
        a.delivery();
    }
}
