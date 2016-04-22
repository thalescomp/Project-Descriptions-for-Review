##Project Overview
For this project, students will answer 5 technical interview questions and get feedback from a qualified reviewer.

##Why This Project?
Having the knowledge to get through technical interviews is certainly helpful, but it won’t mean very much if you can’t clearly demonstrate this knowledge. This project will be assessed for correctness, but also criteria a real interviewer would look for, like clear and clean code, an understanding of efficiency, good communication, et cetera.

##What Will I Learn?
You will learn where your interviewing weaknesses lie. Graders have been instructed to be tough, so you cannot pass unless your answers are good enough that a real interviewer would be impressed.

##How Do I Complete this Project?
1. Make sure you have some prior knowledge of technical interviewing or have gone through the Technical Interviewing course.
2. For each question, create a solution in Java (Java 8). All solutions should be functions named as “question1”, “question2”, et cetera. Code solutions must be in a .java file.
3. Write up an explanation for each question in a single separate text (.txt) or markdown (.md) file. Your paragraph should not be a detailed walkthrough of the code you provided, but provide your reasoning behind decisions made in the code. For example, why did you use that data structure? You also need to explain the efficiency (time and space) of your solution.
4. Compress your one Java and one text file into a .zip, and submit on the website.

Here are the questions:

1. Given two strings `s` and `t`, determine whether some anagram of t is a substring of s. For example: if s = “udacity” and t = “ad”, then the function returns True. Your method signature should look like: `public static boolean question1(String s, String t)`.
2. Given a string `a`, find the longest palindromic substring contained in `a`. Your method signature should look like: `public static String question2(String a)`.
3. Given a graph `G`, find the minimum spanning tree within `G`. A minimum spanning tree connects all vertices in a graph with the smallest possible total weight of edges. Your method should take in and return an adjacency list. Vertices are represented as unique strings. The method signature should be `public static HashMap<String, ArrayList<EdgeAdj>> question3(HashMap<String, ArrayList<EdgeAdj>> G)`. The `EdgeAdj` class is defined as follows: 
```Java 
class EdgeAdj {
String node;
int weight;

public EdgeAdj(String node, int weight) {
this.node = node;
this.weight = weight;
}
}
```

4. Find the least common ancestor between two nodes on a binary search tree. The least common ancestor is the farthest node from the root that is an ancestor of both nodes. For example, the root is a common ancestor of all nodes on the tree, but if both nodes are descendents of the root's left child, then that left child might be the lowest common ancestor. You can assume that both nodes are in the tree, and the tree itself adheres to all BST properties. The function definition should look like `public static int question4(int[][] T, int r, int n1, int n2)`, where T is the tree represented as a matrix, where the index of the list is equal to the integer stored in that node and a 1 represents a child node, r is a non-negative integer representing the root, and n1 and n2 are non-negative integers representing the two nodes in no particular order. For example, one test case might be 
```Java
int[][] T = {{0,1,0,0,0},{0,0,0,0,0},{0,0,0,0,0},{1,0,0,0,1},{0,0,0,0,0}};
question4(T,3,1,4);
```
, and the answer would be 3.
5. Find the element in a singly linked list that's n elements from the end. For example, if a linked list has 5 elements, the 3rd element from the end is the 3rd element. The method signature should look like `public static int question5(Node head, int n)`, where head is the first node of a linked list and n is the "nth number from the end". You should copy/paste the Node class below to use as a representation of a node in the linked list. Return the value of the node at that position.

```Java
class Node {
int data;
Node next;

public Node(int data) {
this.data = data;
}

public Node(int data, Node next) {
this.data = data;
this.next = next;
}
}
``` 

##Evaluation
Your project will be evaluated by a Udacity Code Reviewer according to the rubric here. All criteria must "meet specifications" in order to pass.
