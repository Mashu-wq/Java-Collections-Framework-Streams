# Java-Collections-Framework & Streams

## ArrayList
An arrayList is a resizable array implementation of the list interface. Unlike arrays in Java, which have a fixed size, an arrayList can change its size dynamically as elements are added or removed. 

```
int [] arr = new int[10] //array declaration which has fixed size
ArrayList<Integer> list = new ArrayList<>(); //ArrayList declaratio which has dynamic size
```
```
//list creation
list.add(1)
list.add(2)
list.add(80)
System.out.println(list.get(2)); // will display the value which is positioned in index 2. OUTPUT: 80
System.out.println(list.size()); // returns the array size, OUTPUT: 3
for(int i = 0; i < list.size(); i++){
System.out.println(list.get(i)); // 1, 2, 80
}
//using collection
for(int x: list){
System.out.println(x); // 1, 2, 80
}
System.out.println(list.contains(5)); // False
System.out.println(list.contains(2)); // True
```
```
list.remove(2);// remove the value of 2 index -> 1, 2
```
```
list.add(2, 50); //first is index no and second is value -> 1, 2 , 50
list.set(1,8) // set will replace the 1 index value -> 1, 8, 50
```
```
//Default constructor, creates an empty ArrayList with an initial capacity of 10
ArrayList<String> list = new ArrayList<>();

//Creating an ArrayList with a specified intial capacity
ArrayList<String> listWithCapacity = new ArrayList<>(20);

//Creating an ArrayList from another collection
List<String> anotherList = Arrays.asList("A", "B", "C");
ArrayList<String> listFromCollection = new ArrayList<>(anotherList);
//To show the className use `list.getClass().getName()`
```
```
ArrayList<Integer> list = new ArrayList<>();
list.add(1);
list.add(2);
list.add(3);
list.add(0, 0);
List<Integer> list1 = List.of(4, 5, 6, 7); // Immutable
list.addAll(list1)
System.out.println(list); // 1, 2, 3, 4, 5, 6, 7
```
```
list.remove(1); // remove 1 index value -> 1, 3
list.remove(Integer.valueOf(1)); // remove the value 1 -> 2, 3
```
```
String [] array = list.toArray(new String[0]); // converting to Array
```










