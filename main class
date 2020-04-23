package projectdata;

import java.util.Scanner;


public class Projectdata {

    
    
    public static void main(String[] args) {
       
        BST tree = new BST();
 
          boolean x = true;
          
          
          while(x){
              
              Scanner input = new Scanner(System.in);
              System.out.println("Enter Number 1 to add the dictionary");
              System.out.println("Enter Number 2 to add a word ");
              System.out.println("Enter Number 3 to Search for a word "); 
              System.out.println("Enter Number 4 for preOrder Traversal");
              System.out.println("Enter Number 5 for inOrder Traversal");
              System.out.println("Enter Number 6 for postOrder Traversal");
              System.out.println("Enter Number 7 for BFS Traversal");
              System.out.println("Enter Number 8 to Know the Size of the tree");
              System.out.println("Enter Number 9 to Know the Height of the Tree");                         
              System.out.println("Enter Number 10 to Exit");
              System.out.println("-----------------------------");
              int z = input.nextInt();
              
              switch(z)
              {
                             
                  case 1 :   
                      
                                        String di []={"correctible","fisher-cat","tool-demagnetizer","firstling","prudentiality","nondangerous","limsy","silver-tuned","sea-kindliness","monger"

,"distinguishably","prefertilize","switchman","yarm","schoolyard","bedribble","Ateba","nonexcepted","phasmatrope","odontoid","tallow-face"

,"immense","birdweed","hopoff","Mongolize","net-assets","perfusion","completively","shallowhearted","inure","life-history","ambuling","essayist","suprathoracic"

,"skiametry","town-guard","endorachis","net-silk","phonotypist","tail-pipe","concurringly","uncondensable","little-regarded","Spigelian"

,"unbarreled","clay-tempering","cocuisa","undeparted","six-faced","taboret","lake-moated","philopatrian","degenerately","postatrial"

,"Gaullist","epithelioma","braeface","porridgelike","obituary","unprocessed","acier","Lamium","Lepilemur","hoodlumize","trabant","strong-looking"

,"disincarnation","cameralistic","fluellen","unbuyable","Grendel","paradiplomatic","strawberrylike","misosophist","pseudoetymological"

,"romanticism","segregable","twice-terminated","ploratory","metroclyst","scops-owl","akule","apprehender","Bahima","scrota","bellmaster"

,"exorableness","underworker","spinach-dock","turbid","ten-mile","triglandular","unperjured","twaddling","drainage-pipe","still-burn","reticule","paradenitis","zygadenine"};
          
          
          
          
          for (int i = 0 ; i < di.length ; i++){   
           tree.add(di[i]);
          }
                      
              break; 
              
                 case 2 :    
                      String newword = input.next();
                      tree.add(newword);
                      break;
                      
                      case 3 :            
                    System.out.println("Enter the word to find if it exists or not");
                    String word = input.next();
                    tree.searchAndInsert(word, tree.root);                 
                    break;
                  
                  
                  case 4 :
                      System.out.println("Print in preOrder Traversal");
                      tree.preOrder(tree.root);
                      System.out.println("---------------------------");
                      break;
                      
                  case 5:
                      System.out.println("Print in inOrder Traversal");
                      tree.inOrder(tree.root);
                      System.out.println("---------------------------");
                      break;
                      
                  case 6 :
                      System.out.println("Print in postOrder Traversal");
                      tree.postOrder(tree.root);
                      System.out.println("---------------------------");
                      break;
                      
                      
                  case 7 :
                      System.out.println("Print in BST Traversal");
                      tree.BFS(tree.root);
                      System.out.println("---------------------------");
                      break; 
                      
                  case 8 :
                      System.out.println("The Size of the Tree is   " + tree.size);      
                      System.out.println("---------------------------");
                      break;
                  
                  
                  case 9 :
                      System.out.println("The height of the Tree is   " + tree.height(tree.root));
                      System.out.println("---------------------------");
                      break;

                  
                  case 10 :    
                      x = false;
                      break;
                      
                  default :
                      System.out.println("Wrong Answer , Try Again");
                      break;
      
              }
     
          }
          

        
    }
    
}
