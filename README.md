# LinkedList_Histogram

## Lab Description :   
Write a program that uses nodes to store letters and letter counts.  The data structure created for this program is similar to a Map.   Each node will store a character, a count of how many of those characters have occurred, and a reference to the next node in the list.  Each character with its count will occur at most once in the list

## HistoNode 
– stores a letter, the letter’s count, and the next node

```
public class HistoNode
{
   private char letter;
   private int letterCount;
   private HistoNode next;

   public HistoNode(char let, int cnt, HistoNode n){
	letter=let;
	letterCount=cnt;
	next=n;
   }

   public char getLetter(){
	return letter;
   }

   public int getLetterCount(){
	return letterCount;
   }

   public void setLetter(char let){
	letter=let;
   }

   public void setLetterCount(int cnt){
	letterCount=cnt;
   }

   public void setNext(HistoNode n){
      next = n;
   }
}
```

## Sample Data
```
A A A A B V S E A S A A 
A B C
A B C A B C A B C A B C A B C
```

## Sample Output
```
E - 1     S - 2     V - 1     B - 1     A - 7
C - 1     B - 1     A - 1
C - 5     B - 5     A - 5

```

