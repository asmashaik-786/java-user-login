#CODE FOR USER REGNO:


package commm;
import java.util.Scanner;
import java.util.ArrayList;
public class regg {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Userreg(sc);
    }
    public static String Userreg(Scanner sc) {
        System.out.println("Enter your First Name:");
        sc.next();
        System.out.println("Enter your second name:");
        sc.next();
        System.out.println("Enter your mobile number");
        validatemobile(sc);
        System.out.println("Enter your gender");
        sc.next();
        System.out.println("Enter your password");
        String password=validatepassword(sc);
        System.out.println("Enter your email address");
        String email=validateemail(sc);
        System.out.println("submit");
		return null;
    }
    protected static String validatepassword(Scanner sc) {
        int weak = 0;
        int medium = 0;
        int medium2 = 0;
        int strong = 0;
        boolean f = false;
        while (true){
            String s4 = sc.nextLine();
            for (int i = 0; i < s4.length(); i++) {
                if (s4.charAt(i) >= 'a' && s4.charAt(i) <= 'z') {
                    weak = 1;
                } else if (s4.charAt(i) >= 'A' && s4.charAt(i) <= 'Z') {
                    medium = 1;
                } else if (s4.charAt(i) >= '0' && s4.charAt(i) <= '9') {
                    medium2 = 1;
                } else {
                    strong = 1;
                }
            }
            int c = weak + medium + medium2 + strong;
            if (c == 3 || c == 4) {
                System.out.println("You have a strong password");
                f = true;
                break;
            } else {
                System.out.println("Please enter a strong password");
            }
        }
        return null;
    }
    private static String validatemobile(Scanner sc) {
        boolean f = false;
        while (true) {
            String number = sc.next();
            if (number.matches("\\d{10}")) {
                f = true;
                break;
            } else {
                System.out.println("Please enter a valid number");
            }
        }
        if (f) {
            System.out.println("Okay, it is a valid number");
        }
        return null;
    }
    protected static String validateemail(Scanner sc) {
    while (true) {
        ArrayList<Character> a1 = new ArrayList<>();
        String s3 = sc.next();
        for (int i = 0; i < s3.length(); i++) {
            if (s3.charAt(i) == '@') {
                a1.add(s3.charAt(i + 1));
            }
        }
        boolean f = false;
        if (a1.size() == 1) {
        	for (int i = 0; i < a1.size(); i++) {
                if (a1.get(i) >= 'a' && a1.get(i) <= 'z') {
                    f = true;
                    break;
                }
            }
        }
        if (f) {
            System.out.println("Okay, it is a valid email");
        } else {
            System.out.println("Please enter a valid email address");
        }
        a1.clear();
    }
   }
}
CODE FOR LOGIN 


package commm;
import java.util.Scanner;
import java.util.ArrayList;
public class regg {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Userreg(sc);
    }
    public static String Userreg(Scanner sc) {
        System.out.println("Enter your First Name:");
        sc.next();
        System.out.println("Enter your second name:");
        sc.next();
        System.out.println("Enter your mobile number");
        validatemobile(sc);
        System.out.println("Enter your gender");
        sc.next();
        System.out.println("Enter your password");
        String password=validatepassword(sc);
        System.out.println("Enter your email address");
        String email=validateemail(sc);
        System.out.println("submit");
		return null;
    }
    protected static String validatepassword(Scanner sc) {
        int weak = 0;
        int medium = 0;
        int medium2 = 0;
        int strong = 0;
        boolean f = false;
        while (true){
            String s4 = sc.nextLine();
            for (int i = 0; i < s4.length(); i++) {
                if (s4.charAt(i) >= 'a' && s4.charAt(i) <= 'z') {
                    weak = 1;
                } else if (s4.charAt(i) >= 'A' && s4.charAt(i) <= 'Z') {
                    medium = 1;
                } else if (s4.charAt(i) >= '0' && s4.charAt(i) <= '9') {
                    medium2 = 1;
                } else {
                    strong = 1;
                }
            }
            int c = weak + medium + medium2 + strong;
            if (c == 3 || c == 4) {
                System.out.println("You have a strong password");
                f = true;
                break;
            } else {
                System.out.println("Please enter a strong password");
            }
        }
        return null;
    }
    private static String validatemobile(Scanner sc) {
        boolean f = false;
        while (true) {
            String number = sc.next();
            if (number.matches("\\d{10}")) {
                f = true;
                break;
            } else {
                System.out.println("Please enter a valid number");
            }
        }
        if (f) {
            System.out.println("Okay, it is a valid number");
        }
        return null;
    }
    protected static String validateemail(Scanner sc) {
    while (true) {
        ArrayList<Character> a1 = new ArrayList<>();
        String s3 = sc.next();
        for (int i = 0; i < s3.length(); i++) {
            if (s3.charAt(i) == '@') {
                a1.add(s3.charAt(i + 1));
            }
        }
        boolean f = false;
        if (a1.size() == 1) {
        	for (int i = 0; i < a1.size(); i++) {
                if (a1.get(i) >= 'a' && a1.get(i) <= 'z') {
                    f = true;
                    break;
                }
            }
        }
        if (f) {
            System.out.println("Okay, it is a valid email");
        } else {
            System.out.println("Please enter a valid email address");
        }
        a1.clear();
    }
   }
}
