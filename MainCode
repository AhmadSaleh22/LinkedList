package linkedlist;
public class LinkedList {
    public static void print(Node node1){
        Node N=node1;
        while(N!=null){
            System.out.println(N.info);
            N=N.link;
        }
    }
    public static void InsertAfter(Node PrevNode,int info){
        Node NewNode=new Node(info);
        if(PrevNode.link!=null){
        NewNode.link=PrevNode.link;
        PrevNode.link=NewNode;}
        else
            PrevNode.link=NewNode;
        
    }
    public static void DeleteNode(int key,Node Head){
        Node temp = Head, prev = null; 
  
        // If head node itself holds the key to be deleted 
        if (temp != null && temp.info == key) 
        { 
            Head = temp.link; // Changed head 
            return; 
        } 
  
        // Search for the key to be deleted, keep track of the 
        // previous node as we need to change temp.next 
        while (temp != null && temp.info != key) 
        { 
            prev = temp; 
            temp = temp.link; 
        }     
  
        // If key was not present in linked list 
        if (temp == null) return; 
  
        // Unlink the node from linked list 
        prev.link = temp.link; 
            
    }
    public static void main(String[] args) {
        Node Head=new Node(4);
        Node second=new Node(55);
        Node third=new Node(7);
        Head.link=second;
        second.link=third;
        InsertAfter(second,99);
        print(Head);
    }
    
}
