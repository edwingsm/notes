# Map and Collection

![Exception Hireacrchy](map_and_collection.jpg "map_and_collection.jpg")

![Collection Tree Diagram](collection_tree_diagram.jpg "collection_tree_diagram.jpg")

## SET vs LIST

![Exception Hireacrchy](list_vs_set.jpg "list_vs_set.jpg")

![Exception Hireacrchy](list_vs_set2.jpg "list_vs_set2.jpg")

- <http://www.java67.com/2013/06/how-get-method-of-hashmap-or-hashtable-works-internally.html>

## List Vs Set Vs Queue

In brief:

- A list is an ordered list of objects, where the same object may well appear more than once. For example: [1, 7, 1, 3, 1, 1, 1, 5]. It makes sense to talk about the "third element" in a list. You can add an element anywhere in the list, change an element anywhere in the list, or remove an element from any position in the list.

- A queue is also ordered, but you'll only ever touch elements at one end. All elements get inserted at the "end" and removed from the "beginning" (or head) of the queue. You can find out how many elements are in the queue, but you can't find out what, say, the "third" element is. You'll see it when you get there.

- A set is not ordered and cannot contain duplicates. Any given object either is or isn't in the set. {7, 5, 3, 1} is the exact same set as {1, 7, 1, 3, 1, 1, 1, 5}. You again can't ask for the "third" element or even the "first" element, since they are not in any particular order. You can add or remove elements, and you can find out if a certain element exists (e.g., "is 7 in this set?")

| *HashMap*       | *LinkedHashMap*           | *TreeMap*  |
| ------------- |-------------| -----|
| Extends AbstractMap class. | Extends HashMap class. | Extends AbstractMap class. |
| Implements Map interface. | Implements Map interface. | Implements NavigableMap and SortedMap interfaces. |
| Provide constant time performance for ‘get’ and ‘put’ operations.  | Implementation of Hash Table and Linked List. | Underlying data structure is Red-Black Tree. |
| No Iteration Order. | Maintains a doubly-linked list | Insertion order is not maintained. |
| Key can be null. | Iteration takes place in the order in which the entries were put into the map. | Sorted according to the natural order of keys. |
| Value can be null.   | Fail-fast. | Fail-fast behavior is not guaranteed always. |
| Fail-fast. | Key can be null. | Key can’t be null; if it’s null,  java.lang.NullPointerException occurs.  |
| Duplicate keys are not allowed. | Value can be null. | Keys must be of same type; if not,  java.lang.ClassCastException occurs. |
| Implementation is not synchronized. | Duplicate keys are not allowed. | Value can be null. |
| |Implementation is not synchronized. |Duplicate keys are not allowed. |
|||Implementation is not synchronized.
