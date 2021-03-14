import java.util.Scanner;

public class Solution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int v = sc.nextInt();
        int t = sc.nextInt();
        int s = v * t;
        if (s > 0) {
            System.out.println(s % 109);
        } else if (s <= 0) {
            int a = 109 + (s % 109) % 109;
            if (a == 109) {
                System.out.println(0);
            } else {
                System.out.println(a);
            }
        }
    }
}
