import java.util.ArrayList;
import java.util.List;

class Ride {
    String name;
    String pickup;
    String drop;
    double fare;
    List <String> stops;
    String status;
    Ride(String name, String pickup, String drop){
        this.name=name;
        this.pickup=pickup;
        this.drop=drop;
        this.stops=new ArrayList<>();
        this.status="BOOKED";
        this.fare=calculateFare();
    }
    Ride(String name, String pickup, String drop, List<String> stops){
        this.name=name;
        this.pickup=pickup;
        this.drop=drop;
        this.stops=new ArrayList<>(stops);
        this.status="BOOKED";
        this.fare=calculateFare();
    }
    double calculateFare(){
            return 50+(stops.size()*50);
    }
    void showDetails(){
        System.out.println("--------------------------------");
        System.out.println("Name: "+this.name);
        System.out.print("Route: "+this.pickup);
        for(String s: stops){
            System.out.print(" --> "+s);
        }
        System.out.println(" --> "+this.drop);
        System.out.println("Fare: Rs. "+this.fare);
        System.out.println("Status: "+this.status);
        System.out.println("--------------------------------");
    }
    void cancelRide(){
        if(this.status.equals("CANCELLED")){
            System.out.println("Already cancelled");
        }
        else if(this.status.equals("COMPLETED")){
            System.out.println("Completed ride cannot be cancelled");
        }
        else{
            this.status="CANCELLED";
            this.fare=0;
            System.out.println("Successfully Cancelled");
        }
    }
    void completeRide(){
        if(this.status.equals("COMPLETED")){
            System.out.println("Already completed");
        }
        else if(this.status.equals("CANCELLED")){
            System.out.println("Cancelled ride cannot be completed");
        }
        else{
            this.status="COMPLETED";
            System.out.println("Successfully completed");
        }
    }
}
public class RideBookingApp{
    public static void main(String[] args) {
        Ride R1= new Ride("Rahul","Anna Nagar","Guindy");
        R1.showDetails();
        R1.cancelRide();
        R1.cancelRide();
        R1.showDetails();
        List<String> stops=new ArrayList<>();
        stops.add("T Nagar");
        stops.add("Tambaram");
        Ride R2=new Ride("Angeline", "Anna Nagar", "Guindy", stops);
        R2.showDetails();
        R2.completeRide();
        R2.cancelRide();
        R2.showDetails();
    }
}
