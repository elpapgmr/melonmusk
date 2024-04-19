import java.util.Date;

public class SimpleClock {
    public static void main(String[] args) {
        while (true) {
            Date currentTime = new Date();
            System.out.println("Current time: " + currentTime);
            
            // Wait for 1 second before displaying the time again
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
    }
}
