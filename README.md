# ArrayListRemoveEveryOther
ArrayListRemoveEveryOther
public static void main(String[] args) {
		/*
		 * Create a method that:
		 * is called removeEveryOther
		 * returns nothing
		 * takes in a single parameter - an ArrayList of Strings called words
		 * This method should take the ArrayList parameter and 
		 * modify it by removing every other element in the list, 
		 * starting with removing the 0th element.
		 * For example, if the parameter is:
		 * ("hi","yo","sup","yolo","boop")
		 * The modified ArrayList should be:
		 * ("yo","yolo")
		 */
		ArrayList<String> list = new ArrayList<String>();
		list.add("hi");
		list.add("yo");
		list.add("sup");
		list.add("yolo");
		list.add("boop");
		
		
	
		removeEveryOther(list);
		

	} public static void removeEveryOther(ArrayList<String> words) {
		for(int z=0; z<words.size(); z++) {
			if(z%2==0) {
				words.remove(words.get(z));	
			} 
			if(z%2!=0) {
			words.remove(words.get(z));
			}
		}
		System.out.println(words);
	
	}

}
