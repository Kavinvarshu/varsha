import java.util.ArrayList;
import java.util.Scanner;
class Timetable {
	public static void main(String []args) {
		String[] days = {"Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"};
		String[] times = {"09:00 - 10:00", "10:00 - 11:00", "11:00 - 12:00", "12:00 - 01:00", "01:00 - 01:45", "01:45 - 02:40", "02:40 - 03:35", "03:35 - 04:30"};
		ArrayList<String> subjects = new ArrayList<String>();
		Scanner scanner = new Scanner(System.in);
		int index = 0;
		System.out.println("*** Timetable creator ***");	
		for(String day : days) {
			System.out.println("\n# Routine for " + day + "\n");
			for(String time : times) {
				System.out.println(time);
				String input = scanner.nextLine();
				subjects.add(input);
			}
		}	
		for(String day : days) {
			System.out.println("\n# Routine for " + day + "\n");
			for(String time : times) {
				System.out.println(time + " : " + subjects.get(index));
				index++;
			}
		}	
		scanner.close();
	}
}
@Kavinvarshu
Comment
