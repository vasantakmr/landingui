---
title: Collection Framework
description: Collection Framework
weight: 24
lastmod: 2022-11-20T10:23:30-09:00
draft: false
vimeo: 773628507
emoji: 🚔
video_length: 1:53
free: true
---


#### 1) What is collections framework ?

A framework is set of classes and interfaces to build a functionality. Java collections framework provides 
set of interfaces and classes for storing and manipulating collections. Collection framework contains 
classes and interfaces in java.util package and java.util.concurrent packages.

Advantages or benefits of Collections framework :
1) High performance
2) Using this framework we can create different types of collections
3) We can create our own collection and we can extend a collection.
4) Reduces programming effort.
5) Increases speed and quality : Collections framework provides high performance, implementations of useful data structures and algorithms.

#### 2) What is collection ?

A collection is a container which holds group of objects. Collection provides a way to manage objects easily. Collections manages group of objects as single unit.

Examples include list of strings, integers etc.
Here are few basic operations we do on collections :
1) Adding objects to collection.
2) Removing or deleting objects from collection.
3) Retrieving object from collection.
4) Iterating collection.

#### 3) Difference between collection, Collection and Collections in java?

collection : represent group of objects where objects are stored.
Collection : This is one of the core interface which provides basic functionality for collection.
Collections : Collections contains some utility static methods that operate on collections.

#### 4) Explain about Collection interface in java ?

Collection is the fundamental and root interface in Collections framework. Collection extends Iterable 
interface and inherits iterator method which returns Iterator object.

Signature : 
public interface Collection<E> extends Iterable<E> {
}
Methods in Collection interface :
boolean add(E e); Adds an element to the collection. Returns true if element is added.
boolean remove(Object o);
Removes an object from collection if that object is present in collection. Return true if matching object is removed from collection.
 boolean 
addAll(Collection<? 
extends E> c);
Adds all the elements specified in the collection to this collection.Returns true 
if all elements are added.
boolean 
removeAll(Collection<?> 
c);
Removes all the elements from this collection that are specified in other 
collection.Returns true if all the elements are removed.
int size(); Returns number of elements in collection.
boolean isEmpty(); Checks whether collection contains elements or not. If no elements are 
present it returns false.
boolean contains(Object 
o);
Checks whether specified object is in collection or not. Return true if object is 
in collection.
Iterator<E> iterator(); Used to iterator over collection. No guarantee on order of elements iterated.
boolean 
retainAll(Collection<?> 
c);
Removes all the elements which are not in specified collection. Returns only 
elements specified in collection removing other elements.
Object[] toArray(); Returns an array of elements in collection.


#### 5) List the interfaces which extends collection interface ?

1) List
2) Set
3) Queue
4) Deque ( From Java 6)

#### 6) Explain List interface ?

List interface extends collection interface used to store sequence of elements in collection.
We can even store duplicate elements in list.
We can insert or access elements in list by using index as we do in arrays.
 List is an ordered collection.
The main difference between List and non list interface are methods based on position.

Some of the operations we can perform on List :
1) Adding an element at specified index.
2) Removing an element at specified index.
3) To get the index of element
List contains some specific methods apart from Collection interface methods.

#### 7) Explain methods specific to List interface ?

boolean addAll(int index, Collection<? extends E> c);

This method inserts all the elements in specified 
collection to the list at specified position.

E get(int index); This method returns an element at specified 
position in the list.

E set(int index, E element); This method replaces the element at specified 
position in the list with the specified element.

void add(int index, E element); This method inserts the specified element with the index specified.

E remove(int index); This method removes the element at specified index and returns the element removed.

int indexOf(Object o); indexOf() method returns the index of last occurrence of specified element. If there is no element in the list it removes the element.

ListIterator<E> listIterator(); Returns a list iterator of elements in list.

List<E> subList(int fromIndex, int toIndex); This method returns list of elements between indexes specified.

#### 8) List implementations of List Interface ?

1) ArrayList
2) Vector
3) LinkedList

#### 9) Explain about ArrayList ?

ArrayList is an ordered collection which extends AbstractList and implements List interface.
We use ArrayList mainly when we need faster access and fast iteration of elements in list.
We can insert nulls in to arraylist.
Arraylist is nothing but a growable array.

public class ArrayList<E> extends AbstractList<E> implements List<E>, 
RandomAccess, Cloneable, java.io.Serializable{}

From java 1.4 ArrayList implements RandomAccess interface which is a marker interface which supports fast and random access.

Advantages :
1) Faster and easier access.
2) Used for Random access of elements.
Drawbacks :
1) We cannot insert or delete elements from middle of list.

#### 10) Difference between Array and ArrayList ?

Arrays are used to store primitives or objects of same type or variables that are subclasses of same type.
ArrayList : It is an ordered collection which grows dynamically.
In list we can insert nulls values and list allows duplicate elements.

 ARRAY ARRAY LIST
1) While creating array we have to know the 
size.
1) But it is not required to know size while 
creating ArrayList, because arraylist grows 
dynamically.
2) To put an element in to array we use the 
following syntax :String array[] = 
newString[5];array[1] = “java”;We must know 
specific location to insert an element in to 
2) We can add element to arraylist with following 
syntax :List<String> stringList = new 
ArrayList<String>();stringList.add(“java”);
array. If we try to put element in index which is 
out of range we get ArrayIndexOutOfBounds 
Exception
3) Arrays are static 3) ArrayList is dynamic
4) We can store objects and primitives 4) We can store only primitives prior to 1.5 . From 
1.5 we can store even objects also.
5) We have to manually write logic for inserting 
and removing elements.
5) Just a method call would add or remove 
elements from list.
6) Arrays are faster 6) Arraylist is slower.
7) Arraylist is implemented using arrays.


#### 11) What is vector?

Vector is similar to arraylist used for random access.
Vector is a dynamic array like arraylist.
vector size increases or decreases when elements are added and removed .
Vector is synchronized .
vector and Hashtable are the only collections since 1.0.
Rest of the collections are added from 2.0.
public class Vector<E>extends AbstractList<E>implements List<E>, RandomAccess, Cloneable, java.io.Serializable

#### 12) Difference between arraylist and vector ?

Both ArrayList and vector grows dynamically. The differences between arraylist and vector are :
1) Arraylist is not synchronized and vector is synchronized.
2) Vector is legacy collection introduced in 1.0 and Arraylist introduced in java 2.0.

Performance wise it is recommended to use arraylist rather than vector because by default vector is synchronized which reduces performance if only one thread accesses it.

#### 13) Define Linked List and its features with signature ?

Linked list is used for storing a collection of objects that allows efficient addition and removal of elements in the middle of the collection.

The main drawback with arrays is if we want to insert an element in the middle of the list we need to move each element to next position and insert the element. Similarly with remove if we want to remove an element we need to remove the element and move the list of elements.

But with linked list we can insert and delete in the middle of the list efficiently by just updating the neighbouring node reference.
Linked list class is in java.util package.
Linked List class extends class extends AbstractSequentialList and I mplements List, Deque, Cloneable and Serializable.

Signature :public class LinkedList<E> extends 
AbstractSequentialList<E>
 implements List<E>, Deque<E>, Cloneable, java.io.Serializable
{
}

Important methods specific to LinkedList class :
1) public E getFirst() : getFirst() will returns the first element in the list.

2) public E getLast() : getLast() returns the last element in the list.

3) public E removeFirst() : removeFirst() method removes the first element in the list.

4) public E removeLast() : removeLast() method removes the last element in the list.

5) public void addFirst(E e) : Inserts the element at beginning of the list.

6) public void addLast(E e) :  the element at end of the list.

#### 13) Define Iterator and methods in Iterator?

If we want to iterate through all the elements in collection we use Iterator. Iterator is a standard way to access elements one by one in collection. Iterator is an object associated with collection used to loop 
through the collection.

Steps for accessing elements in Iterator :
1) Obtain Iterator object by calling iterator() method on collection.
Ex : ArrayList <String> al=new ArrayList<String>();
Iterator itr=al.iterator();

2) Call hasNext() method on iterator object in loop as long as hasNext() returns true.
Ex : while(itr.hasNext())
{
}

3) Get each element by calling next() inside the loop.
while(itr.hasNext())
{
String str=itr.next();
}

Methods in iterator :
Method Description
boolean hasNext(); This method returns true if there is next element.hasNext() points to position 
before first element.If there are any elements if will return true.
E next(); Returns the next element in the iteration. . If there are no elements in the 
Iteration NoSuchElementException is thrown. next() will move the pointer to 
next position and returns the element.
void remove(); Removes the element.
Note : If we call next() on last element it will throw java.util.NoSuchElementException. So before calling 
next() first we should call hasNext() whether it has elements or not. If there is next element we can call 
next() so that we can avoid exception.

#### 14) In which order the Iterator iterates over collection?

The order in which Iterator will iterate the collection depends on the traversal order of collection.

For example : for list traversal order will be sequential, and for set the order cannot be determined, and for sorted sorted set will sort the elements in sorted order.
So it all depends on the collection in which order iterator iterates.

#### 15) Explain ListIterator and methods in ListIterator?

List Iterator is similar to Iterator but ListIterator is bidirectional.
We can traverse through the collection in either forward or backward direction.
List Iterator extends Iterator and all the methods in Iterator will be there in ListIterator too with some additional methods .

List Iterator doesn’t have current element .Position of List Iterator lies between two elements i.e previous element and next element.

Features of ListIterator :
1) Traversal of List in either direction.
2) Modification of its elements.
3) Access to elements position.

Signature : 
public interface ListIterator<E> extends Iterator<E> {
}

ListIterator methods :
Method Description

Void add(E obj) Inserts element in to the list infront of the element returned by call to next() and after the element returned by call to next().

boolean hasNext(); Returns true if there are more elements in the list instead of throwing exception if there are no elements.

E next(); Returns the next element . NoSuchElementException is thrown if there is no next element.

boolean hasPrevious(); Returns true if there are elements when iterating list in reverse direction.

E previous(); Returns the previous element in the list.

int nextIndex(); Returns the index of the element returned by next() method. If there are no elements it returns the size of the list.

int previousIndex(); Returns the index of the element returned by previous() method. If there are no elements it returns the size of the list. Returns -1 if the iterator is at beginning of list.

void remove(); Removes the element that was returned by calling next() or previous(). An Illegal state Exception will be thrown if remove() is called before next() or previous().

void set(E e); This method replaces an element in the list with the specified element.

#### 16) Explain about Sets ?

A set is a collection which does not allow duplicates. Set internally implements equals() method which doesn’t allow duplicates. Adding an duplicate element to a set would be ignored. Set interface is implemented in java.util.set package.Set interface does not have any additional methods . It has only collection methods. A set can contain atmost one null value.

ArrayList is an ordered collection.In arraylists order remains same in which they are inserted. But coming to set it is an unordered collection.

public interface Set<E> extends Collection<E> {
}

Important operations that can be performed on set :
1) Adding an element to set.
2) Removing an element from set.
3) Check if an element exist in set.
4) Iterating through set.

#### 17) Implementations of Set interface ?

1) HashSet
2) Linked HashSet
3) TreeSet

#### 18) Explain HashSet and its features ?

Hashset implements set interface and extends AbstractSet. Features of Hashset are :
1) It does not allow duplicates.
2) It does not gurantee ordering of elements.
3) It is unsorted and unordered set.
4) Performance wise it is recommended to use hashset when compared to other sets because it 
internally uses hashing mechanism.
5) Allows insertion of nulls.

Note : For efficiency whenever objects are added to HashSet it need to implement the hashCode() 
method.

public class HashSet<E> extends AbstractSet<E>
implements Set<E>, Cloneable, java.io.Serializable
{
}

#### 19) Explain Tree Set and its features?

TreeSet implements navigableSet interface and extends Abstract set.It creates collection that uses tree for storage.

Features of Treeset are :
1) It does not allow duplicates.
2) When we retrieve the elements in treeset we will get elements in sorted order.

public class TreeSet<E> extends AbstractSet<E>
implements NavigableSet<E>, Cloneable, java.io.Serializable
{}

#### 20) When do we use HashSet over TreeSet?

If we want to search for an element in collection and does not want any sorting order we go for HashSet.

When do we use TreeSet over HashSet?

TreeSet is preferred
1) if elements are to be maintained in sorting order.
2) Fast insertion and retrieval of elements.

#### 21) What is Linked HashSet and its features?

LinkedHashSet extends HashSet and implements Set interface.

public class LinkedHashSet<E> extends HashSet<E> implements Set<E>, Cloneable, java.io.Serializable {
}

Linked HashSet is similar to HashSet but in linked HashSet we maintain order but in HashSet we don’t maintain order. Maintaining order means elements will be retrieved in order which they are inserted.

#### 22) Explain about Map interface in java?
A map is an association of key-value pairs. Both keys and values in map are objects.
Features of map :
1) Maps cannot have duplicate keys but can have duplicate value objects.

#### 23) What is linked hashmap and its features?

LinkedHashMap extends HashMap and implements Map.
Linked hashmap guarantees order of elements . 
Elements are retrieved in same order they are inserted. Linked HashMap uses internally double linked lists to keep insertion order.

The differences between Hashmap and linked hashmap is
1) LinkedHashMap maintains the insertion order while HashMap doesnot maintain order.
2) HashMap if faster for insertion and deletion of elements when compared to linked hashmap. Linked 
hashmap is preferred only for faster iteration of elements.

public class LinkedHashMap<K,V>
extends HashMap<K,V>
implements Map<K,V>
{
}

#### 24) What is SortedMap interface?

SortedMap extends Map interface.Sorted Map maintains sorted order of keys in a map.
By default sorted map maintains natural ordering if we want custom order we can specify using comparator.

public interface SortedMap<K,V> extends Map<K,V> {
}

#### 25) What is Hashtable and explain features of Hashtable?

Hashtable was available before collection framework.
When collection framework was started Hashtable extends Dictionary class and Map interface.
Hashtable offers a convenient way of storing key/ value pairs.
Hashtable does not allow nulls either keys or values.
Hashtable is synchronized.

