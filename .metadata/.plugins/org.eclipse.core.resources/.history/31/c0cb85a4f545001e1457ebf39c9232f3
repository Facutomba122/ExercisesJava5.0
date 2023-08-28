import java.util.ArrayList;
import java.util.Collections;
import java.util.Scanner;

public class CollectionsBasic {

	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		
		ArrayList<String> colorArrayList = new ArrayList<String>();
		colorArrayList.add("rojo");
		colorArrayList.add("verde");
		colorArrayList.add("azul");
		
		//2. Write a Java program to iterate through all elements in an array list
		for (String auxString : colorArrayList) {
			System.out.println(auxString);
		}
		
		//3. Write a Java program to insert an element into the array list at the first position.
		colorArrayList.add(0,"negro");
		
		//4. Write a Java program to retrieve an element (at a specified index) from a given array list
		int i = scanner.nextInt();
		colorArrayList.get(i);
		
		//5. Write a Java program to update an array element by the given element.
		colorArrayList.set(i, "Update");
		
		//6. Write a Java program to remove the third element from an array list.
		colorArrayList.remove(2);
		
		//8. Write a Java program to sort a given array list.
		Collections.sort(colorArrayList);
		
		//9. Write a Java program to copy one array list into another.
		ArrayList<String> auxArrayList = new ArrayList<String>();
		Collections.copy(colorArrayList, auxArrayList);
		
		//10. Write a Java program to shuffle elements in an array list.
		Collections.shuffle(colorArrayList);
		
		//11. Write a Java program to reverse elements in an array list.
		Collections.reverse(colorArrayList);
		
		//12. Write a Java program to extract a portion of an array list.
		
	}
	
	//7. Write a Java program to search for an element in an array list.
	private int searchInArray(ArrayList<String> searchArrayList, String elementSearch) {
		for (String auxString : searchArrayList) {
			if (auxString.equals(elementSearch)) {
				return auxString.indexOf(auxString);
			}
		}
		return -1;
	}
	
	//12. Write a Java program to extract a portion of an array list.
	//assumes that the data types of all ArrayLists are the same
	private ArrayList<?> splitList(ArrayList<?> originalArrayList, int fromIndex, int untilIndex){
		return (ArrayList<?>) originalArrayList.subList(fromIndex, untilIndex);
	}
	
	//13. Write a Java program to compare two array lists. (assumes ArrayList is Integer)
	private boolean compareArrayList(ArrayList<Integer> firstArrayList, ArrayList<Integer> secondArrayList) {
		int maxLength = 0;
		if (firstArrayList.size() > secondArrayList.size()) {
			maxLength = firstArrayList.size();
		} else {
			maxLength = secondArrayList.size();
		}
		
		int[] auxArray = new int[maxLength];
		arrayInizializater(auxArray, 0);
		
		for (int i=0; i<firstArrayList.size(); i++) {
			auxArray[firstArrayList.get(i) % maxLength] += 1;
		}
		
		for (int i=0; i<secondArrayList.size(); i++) {
			auxArray[secondArrayList.get(i) % maxLength] -= 1;
		}
		
		for (int i=0; i<maxLength; i++) {
			if (auxArray[i] != 0) {
				return false;
			}
		}
		return true;
	}
	
	private int[] arrayInizializater(int[] array, int value) {
		for (int i=0; i<array.length; i++) {
			array[i] = value;
		}
		return array;
	}
}
