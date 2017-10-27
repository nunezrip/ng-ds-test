# ng-ds-test

Instructions: create a new repository called ng-ds-test. Within this repo, create a README.md file. Copy and paste all of these questions into this README file and answer them. 
 
Name and describe the two main operations of a stack (to add and remove data). 
 
push(value) - The push() method adds one or more elements to the end of an array and returns the new length of the array. 
 
pop() - The pop method removes the last element from an array and returns that value to the caller. This method changes the length of the array. 
 
Name and describe the two main operations of a queue (to add and remove data). 
 
enqueue() : Adds a node (value)/adds value to the back, returns size 
 
dequeue() : Removes and returns the next node in the queue/removes value from the front, returns size 
 
Draw the tree resulting from adding the following sequence of numbers to an empty tree: 30, 45, 15, 10, 50, 40, 20, 27 
 
                                    ---30--- 
                    ----15---                  ---45--- 
              ----10----                           ----50---- 
          ----20----                                      ---40---   
      ----27---- 
 
                                            ---30--- 
                    ----15---                               ---45--- 
      ----10----          ---- 20---          ---40---         ----50---- 
                                      ---27--- 
 
 


 
 
Is this tree balanced? If not, which rotation needs to be done? (Use the following rotation as an example: rightRotation(30), or leftRotation(10)) 
 
The tree is balanced assuming the value 30 as the root -- A balanced tree is defined as a tree where the depth of all leaf nodes or nodes with single children differ by no more than one. The left and right subtrees' heights differ by one. 
 
rightRotation(30): 
 
                                          ---30--- 
                    ----15---                               ---45--- 
      ----10----          ---- 20---          ---40---         ----50---- 
                                      ---27--- 
 


 
leftRotation(10)): 
 
                                  ---10--- 
                ----15---                             ---20--- 
                                            ---27---                   ----30---- 
                                                                ---40---   
                                                                                        ---45---   
                                                                                                  ---50---   
 


 
 
Now add 29. Is the tree balanced? If not, which rotation needs to be done? (Use the following rotation as an example: rightRotation(30), or leftRotation(10)) 
 
The Tree is NOT balanced. Needs to rotate LEFT on 20 so 27 can become the parent with 20 leaf  left and 29 leaf right. 
 
                                           ---30--- 
                    ----15---                               ---45--- 
      ----10----          ---- 20---          ---40---         ----50---- 
                                        ---27----- 
                                               ---29---  
 


 
                                           ---30--- 
                    ----15---                               ---45--- 
      ----10----          ---- 27---          ---40---         ----50---- 
                       ---20---    ---29----- 
 
 


 
 
Consider the following tree: 
------5 
---2-----8 
-1—3 
 
Now add 0 to the tree. Which one is the first node to go out of balance? 
------5 
---2-----8 
1—3 
0 
 
Node 2 is the first to go out of balance. 
Node 2 needs a right rotation 
Double Rotation: Right Rotation of 2 to bring 3 up and left on 1 to balance the node out and bring 2 to the right 
 
 
How do you fix this node? (Use the following rotation as an example: rightRotation(30), or leftRotation(10)) 
 
---------3 
----1--------5 
0-----2---------8 
 
Fix it with: 
leftRotation(3) to become root. 
RightRoation(2) 
RightRotation(5) 
 
 


 
 
What are the four main steps of mergesort? 
 
Divide 
Sort 
Combine 
Return 
 
Say you have a program which handles the login queue to a game server. The game server is able to log in one person every one second. Assume that one second must elapse after a person logs in with an empty queue before they are removed from the queue. Draw the state of the queue at 12:00:06, considering the following sequence of events: 
 
At 12:00:00 Hades logs in                            
At 12:00:00 Ares logs in                                 
At 12:00:00 Zeus logs in 
At 12:00:00 Buzz Light Year logs in 
At 12:00:02 Kanye West logs in 
At 12:00:03 Taylor Swift logs in 
At 12:00:03 Darkwing Duck logs in 
At 12:00:04 Evil Mickey logs in. 
 
ANSWER: At 12:00:06 you'll have two users waiting. 
 
State at 12:00:06  

At 12:00:00  
01 in 
Hades logs in                          

At 12:00:00  
02 in 
Ares logs in                                 

At 12:00:00  
03 in 
Zeus logs in 

At 12:00:00  
04 in 
Buzz Light Year logs in 

At 12:00:02  
05 in 
Kanye West logs in 

At 12:00:03  
06 in 
Taylor Swift logs in 

At 12:00:03  
07 waiting 
Darkwing Duck logs in 

At 12:00:04  
08 waiting 
Evil Mickey logs in. 
 
Solve https://www.hackerrank.com/challenges/compare-the-triplets - be mindful that you are required to print the output to the console in exactly the format that was asked. You are not required to return a value, just print to the console. Also be mindful to use JavaScript. 
 
/////////////// ignore above this line //////////////////// 
 
 
// Complete this function 
    let A = 0;  
    let B = 0;  
    if (a0 > b0){  
        A += 1;  
    }  
     if (a2 < b2){  
        B += 1;  
     }  
    
    return A+' '+B; 
 
 
Solve https://www.hackerrank.com/challenges/mini-max-sum - be mindful that you are required to print the output to the console in exactly the format that was asked. You are not required to return a value, just print to the console. Also be mindful to use JavaScript. 
