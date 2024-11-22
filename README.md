
/**
 This Java program calculates the largest distance between three points on a 2D plane. The user is prompted to enter the coordinates for three points (x1, y1),(x2, y2),and(x3, y3).
 The program calculates the distance between each pair of points using the formula which calculates distance between points.
 It then compares the three calculated distances and outputs the largest distance. The program uses the Math.sqrt() and Math.pow() functions to compute the square root and square 
 of the differences between coordinates.
 * @Eden Davidov
 * @I.D-208224972
 **/
import java.util.Scanner;
public class Maxline
{
    public static void main(String[] args)
    {
        Scanner scan=new Scanner(System.in);
        System.out.println("enter first point(x1 y1)");
        int x1=scan.nextInt();
        int y1=scan.nextInt();
        System.out.println("enter secend point(x2 y2)");
        int x2=scan.nextInt();
        int y2=scan.nextInt();
        System.out.println("enter third point(x3 y3)");
        int x3=scan.nextInt();
        int y3 = scan.nextInt();
            double d1 = Math.sqrt(Math.pow(x2 - x1, 2) + Math.pow(y2 - y1, 2));
            double d2 = Math.sqrt(Math.pow(x3 - x1, 2) + Math.pow(y3 - y1, 2));
            double d3 = Math.sqrt(Math.pow(x3 - x2, 2) + Math.pow(y3 - y2, 2));
            double maxDistance = Math.max(d1, Math.max(d2, d3));
          System.out.println("The largest distance is: " + maxDistance);
    }
}

