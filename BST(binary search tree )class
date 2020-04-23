package projectdata;



import java.util.LinkedList;
import java.util.Queue;


public class BST {
    
    String s;
static  String succ,pred;     
 int size = 0;
 Node root;
 String n;
 Node x;

  static String m  ;
    public void add(String data , Node node){
        
       
     
      if (data.compareTo(node.data)>0){
         
          if (node.right == null){
               
              node.right=new Node(data);
             
              return;
          }
         
         add(data , node.right);
         
      }    
      
   else  if (data.compareTo(node.data)<0){
          
          
          if(node.left==null){
             node.left=new Node(data);
             
             return;
          }
          
          add(data,node.left);
        
      }
        
    }
    public void add(String data){
             
        
     if (root == null){   
         root = new Node(data);
        
     }else   {       
         add(data,root);
     }
     
        size++;
    }


    
    
    
    
        public String searchAndInsert(String data , Node node){
        
                      
        if (data.compareTo(node.data)==0){
          System.out.println("The word  " +data+ " is Found");
           return node.data;
        }
        else  if (data.compareTo(node.data)>0&& node.right != null ){
                
             searchAndInsert(data,node.right);
           
        } 
       else if (data.compareTo(node.data)<0&& node.left != null ){
           
             searchAndInsert(data,node.left);   
       }

       else  // if ((node.right == null && node.left == null )|| (node.left == null && data.compareTo(node.data) < 0) || ( node.right == null  && data.compareTo(node.data) > 0))            
              
        {        

            m = node.data;   
            System.out.println("the word "+data+ " isnot found");
            System.out.println("Do You Mean  "+m);
            SuccandPred(root,m);
            System.out.println("Successor  "+succ);
            System.out.println("Predcessor  "+pred);
            System.out.println("the word has been added");
            System.out.println("--------------------------");
            add(data);     
        }                 
     return m;  
    }
        
        
        
        public void SuccandPred(Node node, String data) {
		if (node != null) {
			if (node.data.compareTo(data)==0) {
				
				if (node.left != null) {
					Node z = node.left;
					while (z.right != null) {
						z = z.right;
					}
					pred = z.data;
				}
				if (node.right != null) {
				
					Node y = node.right;
					while (y.left != null) {
						y = y.left;
				}
                           	succ = y.data;
	                     	}
                         	} else if (node.data.compareTo(data)>0) {
				
				succ = node.data;
				SuccandPred(node.left, data);
		         	} else if (node.data.compareTo(data)<0) {
		 		
				pred = node.data;
				SuccandPred(node.right, data);
			}
		}
	}


    
    public int height(Node node){
        
        if (node == null)
            return -1;
        
        else {
            
            int leftOfTheRoot = height(node.left);
            int rightOfTheRoot = height (node.right);
             
        if (leftOfTheRoot > rightOfTheRoot ){     
        return (leftOfTheRoot+1);
        }
        else
            return (rightOfTheRoot+1);
        }
                
    }

     public void BFS(Node node){
         
         if (node == null)
             return;
            
         
         Queue <Node> q = new LinkedList<>();
         q.add(node);
        
            while(!q.isEmpty()){
                
             Node current = q.peek();
             System.out.println(current.data);
             if (current.left != null)
                 q.add(current.left);
             if (current.right != null)
                 q.add(current.right);
             
             q.remove();
                
                
            }
 
        }
     
     
     public void preOrder(Node node){
         
      if (node == null)   
          return;
         
      System.out.println(node.data);
      preOrder(node.left);
      preOrder(node.right);
        
     }
     
     public void inOrder(Node node){
         
      if (node == null)   
          return;
         
      
      inOrder(node.left);
      System.out.println(node.data);
      inOrder(node.right);
        
     }
          
      public void postOrder(Node node){
                      
      if (node == null)   
          return;
        
      postOrder(node.left);
      postOrder(node.right);
      System.out.println(node.data);  
     }

}


