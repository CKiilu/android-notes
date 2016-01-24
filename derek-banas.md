#DEREK BANAS VIDEOS

##STACKS AND QUEUES

They are used to complete a task. Thay are like tools which are used and wuickly discarded.

###STACKS vs QUEUEs

A stack only allows access to one item being the last item in the stack while a queue allows access to the
one item being the first item in the queue.

###STACKS

Syntax: String[] stackArray;

Things to set: stacksize, top of stack.

Array.fill(stackname, "-1"); makes all stack items of index -1 nonexistant.

To add items to a stack use a void push function with string as parameter. Use topofstack++ to get the next index 
make the parameter equal to the value at an index of the stack.

To use a stack you need to initialize it(as an array) and create an object instance in the main menu.
To delete all use a loop.

Removing items from a stack uses a pop function which makes the index equal to -1.

display stack uses a peek function which returns stack values.

To push an item onto the stack use the function prefixed by obj name

Sting[] tempString = name.split(" ") Creates a new item every time there is a space between different parts of an array.

###QUEUES

Creating a queue is similar to creating a stack. The difference comes about in using the functions.

Instead of using push, insert is used; instead of pop remove  but peek remains the same.

Use front and rear in array brackets to signify array indexes. Use rear for last and access the first using front.

####PRIORITY QUEUE

Use Integer class to parseInt the parameter being input in an if statemet contained in a for loop.

##LINKED LIST

A link is an object.

Each link has another link in the list.

The LinkedList has only a reerence to the last link added to it.

Public link is used as a constructor  with parameters.

Create a nested class containing the linkList with firstlink as null.

To check if the list is empty use a boolean which references if the link is null.

###ADDING NEW LINKS

A new link created is referenced to the newest link added.Next is assigned the reference to the previous link created.

      Link newLink = new Link(bookName, millionsSold)
      newLink.next = firstLink;
      firstLink = newLink;
      
###REMOVING LINKS

Firstlink is given the value of the current link.

      Link linkreference=firstlink;
      if(!ItsEmpty90){
      firstlink= firstink.next;
      }else{
      syso("empty list");}
      
###CYCLING IN A LIST

Start at the reference stored in the firstlink of the linkedlist. This gets
the references stored in next for every link until next returns null.

      Sample code
      link theLink = firstlink;
      while(thelink!=null){
            thelink.display();
      }
      
The code checks data for the the firstlink reference stored in the linkedlist
and keeps searching until the end unless a match is found.

      Finding function
      
      public link find(String bookname){
            link thelink = firstlink;
            if(!isEmpty()){
                  while(thelink.bookname != bookname){
                        if(thelink.next == null){
                              return null;
                        } else {
                              thelink = thelink.next
                        }
                  } else {
                        syso("Empty linked list")
            }
            
###REMOVING A SPECIFIC LINK

Cycle through all links until match is found. If referenced link stored in the 
linkedlist's firstlink matches store the reference next in firstlink as firstlink.

If a match occurs elsewhere find the link the next equals the reference to remove.
Get the reference name next in the link to remove and assign it to the link above.

      CODE
      public link removelink(String bookname){
            link currentlink = firstlink;
            link previouslink = firstlink;
            
            while(currentlink.bookname != bookname){
                  if(currentlink.next == null){
                        return null;
                  } else {
                        previouslink = currentlink;
                        currentlink = currentlink.next;
                  }
            }
            if(currentlink == firstlink){
                  firstlink = firstlink.next;
            } else {
                  previuslink.next = currentlink.next;
            }
            return currentlink;
      }
      
###DOUBLE ENDED LINKEDLIST

code

      public class DoubleEndedLinkedList{
            Neighbour firstlink;
            Neighbour lastlink;
            
            public void insertinfirstlnkposition(String homeownername, int housenumber){
                  Neighbour newlink = new Neighbour(homeownername, housenumber);
                  if(isEmpty()){
                        lastlink=newlink;
                  } else {
                  fistlink.previous =newlink;
                  }
                  newlink.next=firstlink;
                  firstlink=newlink;
            }
             public void insertinlastlnkposition(String homeownername, int housenumber){
              Neighbour newlink = new Neighbour(homeownername, housenumber);
                  if(isEmpty()){
                        firstlink=newlink;
                  } else {
                  lastlink.next = newlink;
                  newlink.previous = lastlink;
            }
            lastlink=newlink;
      }

###INSERT LIST ITEM AFTER KEY

Use a boolean function with int key as one of the parameters

###INSERTING LIST IN ODDER

Use a list to sort the linkdedlist values in order.

###USING ITERATORS

Use loops to add and remove multiple list items by using null to break folow.
