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
