# 📘 GTU DSA - All Algorithms

A **comprehensive collection** of all algorithms covered in the **SEM-3 DSA (GTU)** syllabus. This repository is a valuable **reference** and **study guide** for students and enthusiasts alike. 

---

**✨ Created by Dhruv Prajapati.**  

---

## 📖 Quick Links to Chapters  

1. [Chapter 1 - Basic Concepts of DSA](#chapter-1---basic-concepts-of-dsa)  
2. [Chapter 2 - String Operations](#chapter-2---string-operations)  
3. [Chapter 3 - Stack and Queue](#chapter-3---stack-and-queue)  
4. [Chapter 4 - Linked List](#chapter-4---linked-list)  
5. [Chapter 5 - Tree](#chapter-5---tree)  

---

### 💡 How to Use  
- 📚 **Browse** through the chapters using the quick links above.  
- 🛠️ **Understand and practice** algorithms for a strong foundation in data structures and algorithms.  
- 🚀 **Contribute** to the repository if you'd like to add or improve content!  

---

Feel free to reach out or contribute to make this repository even better! 😊

---

## 📝 Notes
- Algorithms are written in pseudo-code format for better understanding and adaptability.
- Ensure to practice these algorithms to strengthen your understanding of the basic operations on arrays.
- For real-world coding, implement these algorithms in your preferred programming language.

## Chapter 1 - Basic Concept of DSA

#### Array Operations

1. [Traverse Array](#1-traverse-array---visit-each-element-of-array)
2. [Search element](#2-search-element---there-is-two-type-linear-search-and-binary-search)
3. [Array Insert](#3-array-insert)
4. [Array Mearge](#4-array-mearge)

#### (1) Traverse Array - visit each element of Array
Algorithm Traverse ( Array , size ) {

    step 1 : [ initialize ]
                    i <- 0w
    step 2 : Repeat Steps 3 , 4 while
                    i < size
    step 3 : print Array[i]
    step 4 : i <- i + 1
    step 5 : exit 

}

#### (2) Search element - (there is two type Linear search and Binary Search)

#### (a) Linear Search
Algorithm Linearsearch ( Array, Size, Target ) {

    step 1 : [ initialize ]
                    i <- 0
    step 2 : Repeat Steps up to 
                    while i < size
    step 3 : if ( Array[i]  = = Target )
                     return i
    step 4 : set i <- i + 1
    step 5 : return -1


}

#### (b) Binary Search

Algorithm Binarysearch ( Array , Size , Target ) {

    step 1 : low <- 0
    step 2 : high <- size - 1
    step 3 : Repeat Steps 4 , 5 
                    while low <= high
    step 4 : mid <- (low + high) / 2
    step 5 : if ( Array[ mid ] > Target ) {
                    high <- mid - 1    
                } 
                else if ( Array[ mid ] < Target ){
                    low <- mid + 1 
                }
                else {
                    return mid
                }
    step 6 : return -1

}

#### (3) Array Insert 

Algorithm Insert ( Array, N, Position, Value ) {

    step 1 : [initialize]
                i <- N-1
    step 2 : Repeat step 3,4 while
                i >= Position
    step 3 : Array[i+1] <- Array[i]
    step 4 : i <- i - 1
                [End of Loop]
    step 5 : set N <- N + 1
    step 6 : set Array[Position] <- Value
    step 7 : exit

}

#### (3) Array Insert 

Algorithm Delete ( Array, N, Position ) {

    step 1 : [initialize]
                i <- Position
    step 2 : Repeat step 3 and 4 while
                i < N - 1
    step 3 : Array[i] <- Array[i+1]
    step 4 : i <- i + 1
                [End of Loop]
    step 5 : N <- N - 1
    step 6 : exit
    
}

#### (4) Array Mearge 

Algorithm Delete ( A, A_Size, B, B_Size ) {

    step 1 : [initialize]
                i <- 0 , Index <- 0
    step 2 : Repeat Steps upto 6 while
                I < A_Size
    step 3 : C[Index] <- A[i]
    step 4 : Index <- Index + 1
    step 5 : i <- i + 1
                [End of Loop]
    step 6 : i <- 0
    step 7 : Repeat steps upto 10 while
                i < B_Size
    step 8 : C[Index] <- B[i]
    step 9 : Index <- Index + 1
    step 10 : i <- i + 1
    step 11 : exit 

}## Chapter 2 - String Operations

String manipulation algorithms.

### Operations:
1. [Find string length](#1--finding-length-of-a-string)
2. [Convert to uppercase or lowercase](#2-converting-characters-of-a-string-into-upper-case-and-lower-case) 
3. [Copy a string](#3-copying-a-string)
4. [Append a string](#4-appending-string)
5. [Concatenate two strings](#5-concatenation-of-two-strings-to-form-a-new-string)
6. [Reverse a string](#6-reversing-a-string)
7. [Compare two strings](#7-comparing-strings)
8. [Delete a substring](#8-deletion-of-string)

#### (1)  Finding length of a string

Algorithm Findlength ( str ) {

    step 1 : [initialize]
                i <- 0
    step 2 : Repeat step 3 while 
                str(i) != NULL
    step 3 : i <- i + 1
    step 4 : [initialize]
                length <- i
    step 5 : exit

}

#### (2) Converting Characters of a string into upper case and lower case

#### (a) Algorithm for Converting string to Uppercase

Algorithm Toupper ( str ) {

    step 1 : [initialize]
                i <- 0
    step 2 : Repeat steps 3, 4 while
                str[i] != NULL
    step 3 : if ( str[i] >= 'a' and str[i] <= 'z' ) {
                upper[i] <- str[i] - 32
            }
            else {
                upper[i] <- str[i]
            }
    step 4 : i <- i + 1
    step 5 : upper[i] <- NULL
    step 6 : exit 
}

#### (b) Algorithm for Converting string to Lowercase

Algorithm Tolower ( str ) {

    step 1 : [initialize]
                i <- 0
    step 2 : Repeat steps 3, 4 while
                str[i] != NULL
    step 3 : if ( str[i] >= 'A' and str[i] <= 'Z' ) {
                lower[i] <- str[i] + 32
            }
            else {
                lower[i] <- str[i]
            }
    step 4 : i <- i + 1
    step 5 : lower[i] <- NULL
    step 6 : exit 
}

#### (3) Copying a string

Algorithm Copy ( strSource, strDest ) {

    step 1 : [initialize]
                i <- 0
    step 2 : Repeat step 3,4 while
                strSource[i] != NULL
    step 3 : strDest[i] = strSource[i]
    step 4 : i <- i + 1
    step 5 : strDest[i] <- NULL
    step 6 : exit 

}

#### (4) Appending String

Algorithm Append ( strSource, strDest ) {

    step 1 : [initialize]
                i <- 0, j <- 0
    step 2 : Repeat step 3 while
                strDest[i] != NULL
    step 3 : i <- i + 1
    step 4 : Repeat steps 5, 6, 7 while
                strSource[i] != NULL
    step 5 : strDest[i] <- strSource[j]
    step 6 : i <- i + 1
    step 7 : j <- j + 1
    step 8 : strDest[i] <- NULL
    step 9 : exit

}

#### (5) Concatenation of two strings to form a new string

Algorithm Concate ( str1, str2 ) {

    step 1 : [initialize]
                i <- 0, j <- 0
    step 2 : Repeat steps 3 while str1[i] != NULL
    step 3 : str3[k] = str1[i]
    step 4 : i++, k++
    step 5 : Repeat steps 5 while
                str2[j] != NULL
    step 6 : str3[k] = str2[j]
    step 7 : j++, k++
    step 8 : str3[k] = NULL
    step 9 : exit
}

#### (6) Reversing a string

Algorithm Reverse ( str ) {

    step 1 : [initialize]
                i <- 0
    step 2 : j <- length(Str) - 1
    step 3 : Repeat steps 4, 5, 6 while
                i < j
    step 4 : swap( str[i], str[j] )
    step 5 : i <- i + 1
    step 6 : j <- j + 1
                [End of While]
    step 7 : exit

}

#### (7) Comparing strings

Algorithm Compare( str1, str2 )
{

    step 1 : [initialize]
                i <- 0, same <- 0
    step 2 : set len1 <- length(str1) , len2 <- length(str2)
    step 3 : if len1 != len2 {
                write "String Are not equal"
            }
            else {
                repeat while i < len1 {
                    if str1[i] == str2[i] {
                        set i++
                    }
                    else{
                        go to step 4
                    }
                }
                if i = len1 {
                    set same = 1
                    write "strings are equal"
                }
            }
    step 4 : if same = 0 {
                if str1[i] > str2[i] {
                    write "string 1 is grater then string 2"
                }
                else if ( str1[i] < str2[i] ) {
                    write "string 2 is grater then string 1"
                }

            }
    step 5 : exit
}

#### (8) Deletion of string

Algorithm Delete ( Text, Pos, length ) {

    step 1 : [initialize]
                i <- 0, j <- 0
    step 2 : Repeat steps 3 while 
                Text[j] != NULL
    step 3 : if ( i = Pos ) then
                i <- i + length
            else
                newstr[j] <- Text[i]
                j <- j + 1
                i <- i + 1
                    [end of While]
    step 4 : newstr[j] = NULL
    step 5 exit  

}## Chapter 3 - Stack and Queue

#### Operations of Stack

1. [Push Operation ( Insert element in to Stack )](#a-push-operation-operation)
2. [Pop Operation ( Delete element from Stack )](#b-pop-operation--operation)

#### Operations of Queue

1. [Enqueue Operation ( Insert element in Queue )](#a-enqueue-operation)
2. [Dequeue Operation ( Delete element from Queue )](#b-delete-operation) 
#### Stack Operations
#### (a) Push Operation

Algorithm Push ( Stack, Top, X ) {

    step 1 : [Check Overflow]
            if ( Top >= size - 1 ) then
                write "Stack Overflow"
                return
    step 2 : Top <- Top + 1
    step 3 : Stack[Top] = X
    step 4 : exit 

}

#### (b) Pop Operation

Algorithm Pop ( Stack, Top ) {

    step 1 : [Check Underflow]
            if ( Top == -1 ) then 
                write "Stack Underflow"
                return
    step 2 : [Remove Top Most Element]
            temp <- Stack[Top]
    step 3 : [Decrement Top Pointer]
            Top <- Top - 1
    step 4 : [Return The Value]
            return temp
    step 5 : exit

}

#### Queue Operations
#### (a) Enqueue Operation

Algorithm Qinsert ( Rear, Queue, N, X, Front ) {

    step 1 : [Check Overflow]
            if Rear >= N
                write "Queue is Overflow"
                return
    step 2 : [increment Rear by 1]
                Rear++
    step 3 : [Insert Element at Queue]
                Queue[Rear] <- X
    step 4 : [Check if first time inser done]
            if Front == 0 then   
                Front = 1
    step 5 : exit

}

#### (b) Delete Operation

Algorithm Qelete ( Queue, Rear, Front ) {

    step 1 : [Check Queue is Underflow]
            if Front == 0 then
                write "Qelete is Underflow"
                return
    step 2 : [Delete Front element]
                y = Qelete[Front]
    step 3 : [Update Front Pointer Value]
            [Check if it is 1st element]
            if Front == Rear then
                Front = 0
                Rear = 0
            else
                Front <- Front + 1
    step 4 : return y
    step 5 : exit

}## Chapter 4 - Link List

#### Link List Operations
1. [Insert New Node at the Begining of Link List.](#1-insert-new-node-at-the-begining-of-link-list)
2. [Insert New Node at the end of Link List.](#2-insert-new-node-at-the-end-of-link-list)
3. [Insert New Node After Given Specific Node.](#3-insert-new-node-after-given-specific-node)
4. [Insert New Node Before Given Specific Node.](#4-insert-new-node-before-given-specific-node)
5. [Insert New Node into ordered Link List.](#5-insert-new-node-into-ordered-link-list)
6. [Delete First Node of Link List.](#6-delete-first-node-of-link-list)
7. [Delete Last Node of List Link.](#7-delete-last-node-of-list-link)
8. [Count the Node of Link List.](#8-count-the-node-of-link-list)
9. [Search Specific Node in List List.](#9-search-specific-node-in-list-list)

#### (1) Insert New Node at the Begining of Link List.

Algorithm InsertBeg( First , Value )
{

    Step 1 : [Check For Avaliblity Stack]
                if avail = NULL then
                    write "Available Stack is Empty"
                    return First
    Step 2 : [Obtain address of next free node]
                new <= avail
    Step 3 : [Remove free node from available stack]
                avail <= avail(link)
    Step 4 : [Initialize node to the link list]
                new(info)  <= Value
                new(link)  <= First
    Step 5 : [assign the address of the Temporary Node]
                First <= new
    Step 6 : [finished]
                return First
}

#### (2) Insert New Node at the end of Link List.

Algorithm InsertEnd( first , value )
{
    
    Step 1 : [Check For Avaliblity Stack]
                if avail = NULL then
                    write "Available Stack is Empty"
                    return first
    Step 2 : [Obtain address of next free node]
                new <= avail
    Step 3 : [Remove free node from available stack]
                avail <= avail(link)
    Step 4 : [Initialize node to the link list]
                new(info)  <= value
                new(link)  <= NULL
    Step 5 : [is list is empty?]
                if first = NULL then
                    first <= new
    Step 6 : [initialize search for last node]
                    save <= new
    Step 7 : [search end of the list]
                Repeat while save(link) ` NULL
                    save <= save(link)
    Step 8 : [set link field of last node to new]
                save(link) <= new
    Step 9 : [Finished]
                return first
}

#### (3) Insert New Node After Given Specific Node.

Algorithm InsertAfterPos( value , first , X) {

    Step 1 : [Check for availability stack underflow]
                if avail = NULL then
                    Write “Availability stack underflow”
                    return
    Step 2 : [Obtain address of next free node]
                new <- avail
    Step 3 : [Remove free node from availability stack]
                avail <- link(avail)
    Step 4 : [initialize field of new node]
                info(new) <- X
    Step 5 : [If list is empty?]
                if first = NULL then
                    link(new) <- NULL
                    first <- new
                    return first
    Step 6 : [Search the list until desired address found]
                save <- first
    Step 7 : Repeat while link(save) != NULL 
                    and info(save) !=  value 
    Step 8 : [Insert Node]
                link(new) <- link(save)
                link(save) <- new
    Step 9 : [Finished]
                return(first)
}

#### (4) Insert New Node Before Given Specific Node.

Algorithm InsertBeforePos( value , x , first ) {

    step 1 :- [check availiblity of stack]
                    if avail = NULL then
                        write "Availiblity stack is empty"
                        return
    step 2 :- [obtain address of free node]
                    new  <- avail
    step 3 :- [link avail to next free node]
                    avail <- avail(link)
    step 4 :- [initialize new node]
                    new(info) <- x
    step 5 :- [check linked list is empty?]
                    if first = NULL then
                        new(link) <- NULL
                        first <- new
                        return first
    step 6 :- [check if there is only one node]
                    if first(info) = value then
                        new(link) <- first
                        first <- new
                        return first
    step 7 :- [point save to first]
                    save <- first
    step 8 :- [search for insert node position]
                    pred  <- save
                    save <- save(link)
    step 9 :- [insert new node at position]
                    new(link) <- save
                    pred(link) <- new
    step 10 :- return first
}

#### (5) Insert New Node into ordered Link List.

Algorithm InsertOrder( first , X ) {

    step 1 :- [check availiblity of stack]
                    if avail = NULL then
                        write "Availiblity stack is empty"
                        return
    step 2 :- [obtain address of free node]
                    new  <- avail
    step 3 :- [link avail to next free node]
                    avail <- avail(link)
    step 4 :- [initialize new node]
                    new(info) <- x
    step 5 :- [check linked list is empty?]
                    if first = NULL then
                        new(link) <- NULL
                        first <- new
                        return first
    Step 6 : [does the new node less than all other node]
                    if info(new) <= info(first) then
                        link(new) <- first
                        first <- new
                        return first
    step 7 :- [Search for predecessor of new node]
                    save <= first  
    Step 8 : Repeat while link(save) != NULL and
                    info(link(save)) <= info(new)

                    save <- link(save) 
    Step 9 : [Set link fields of new node and its predecessor]
                link(new) <- link(save)
                link(save) <- New
    Step 10 : return first

}

#### (6) Delete First Node of Link List.

Algorithm delfirst( first ) {

    step 1 :- [check for linked list empty?]
                    if first <= NULL then
                        write "Linked list is empty"
                        return first
    step 2 :- [save data in y]
                    y <- first(info)
    step 3 :- [check there is only one node]
                    if first(link) == NULL then
                        return NULL
    step 4 :-  [initialize temp]
                    temp <- first
    step 5 :- [increment first]
                    first <- first(link)
    step 6 :- [free the node]
                    temp(link) <- avail
                    avail <- temp
    step 7 :- return first
}

#### (7) Delete Last Node of List Link.

Algorithm dellast( first ) {

    step 1 :- [check linked list empty?]
                    if first = NULL then
                        write "Linked list empty"
                        return first
    step 2 :- [check if there is only one  node]
                    if first(link) = NULL then
                        y <- first(info)
                        temp <- first
                        first <- NULL
                        temp(link) <- avail
                        avail <- temp
                        return first
    step 3 :- [initialize save to first]
                    save <- first
    step 4 :- [search for last node]
                    Repeat while save(link) != NULL
                        pred <- save
                        save <- save(link)
    step 5 :-  [delete node]
                    y <- save(info)
                    pred(link) <- NULL
    step 6 :-   save(link) <- avail
                avail <- save
    step 7 :- return first
}

#### (8) Count the Node of Link List.

Algorithm count( first )
{

    Step 1 : [Initialize count to 0] 
                    count <- 0
    Step 2 : [Initialize pointer to first]
                    ptr <- first
    Step 3 :  [Repeat until the end of the list]
                    Repeat steps 4,5 while ptr != NULL
    Step 4 : [Increment the count]
                    count <- count +1
    Step 5 : [Move pointer to the next node]
                    ptr <- ptr(link)
                [End of loop]
    Step 6 : return count
    Step 7 : exit
}

#### (9) Search Specific Node in List List.

Algorithm search( first , target )
{

    Step 1 : [initialize pos and count]
                    pos <= 0, count <= 0
    Step 2 : [initialize pointer to first]
                    ptr <= first
    Step 3 : Repeat steps 4,5
                    while ptr != NULL count <= count + 1
    Step 4 : if ptr(info) = target   then
                    pos = count
                    write "target found"
                    return pos
                    go to step 6
             else
                    ptr <= ptr(link)
    Step 5 : write "target not found"
    Step 6 : exit
}
## Chapter 5 - Tree

#### Tree Traversal Algorithms

1. [Preorder Traversal](#1-preorder-traversal)
2. [Inorder Traversal](#2-inorder-traversal)
3. [Postorder Traversal](#3-postorder-traversal)

#### (1) Preorder Traversal

Algorithm preorder( tree ) {

    step 1 :- [process the root node]
                    if tree != NULL then
                            write "tree->Data"
                    else
                            write "empty data"
                            return
    step 2 :- [process the left subtree]
                    if tree -> lptr != NULL then
                            call preorder(tree->lptr)
    step 3 :- [process the right subtree]
                    if tree->rptr != NULL then
                            call preorder(tree->rptr)

}

#### (2) Inorder Traversal

Algorithm inorder( tree ){
     
    step 1 :- [check for empty tree]
                    if tree = NULL then
                    return
    step 2 :- [process the left subtree]
                    if tree->lptr != NULL then
                        call inorder(tree->lptr)
    step 3 :- write tree->data
    step 4 :- [process the right subtree]
                    if tree->rptr != NULL then
                        call inorder(tree->rptr)
}

#### (3) Postorder Traversal

Algorithm postorder( tree ){

    step 1 :- [check for empty tree]
                    if tree = NULL then
                    return
    step 2 :- [process the left subtree]
                    if tree->lptr != NULL then
                        call inorder(tree->lptr)
    step 3 :- [process the right subtree]
                    if tree->rptr != NULL then
                        call inorder(tree->rptr)
    step 4 :- write tree->data
}