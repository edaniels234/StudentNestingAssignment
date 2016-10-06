# Array Exercises

## User Network

Our User, Joey Plain, has just signed up for Facebook!  
He's very excited and wants to start building out his network as quickly as possible  -and we're going to help him get started.

**Don't mess with lines 1 through 35.**

They are used to create Joey's user object (joeyProfile),  
and the network of all users on Facebook (allUsers).  
We're going to use allUsers to help him find his friends, family, and coworkers.

1) First, let's inspect joeyProfile and allUsers to see what we have.

* [ ] console.dir the joeyProfile object.  
   It should have friends, family, and coworkers arrays.

* [ ] console.dir the allUsers collection.  
   It should have > 20 objects with the same properties as your joeyProfile object.

2) Next, let's add some friends to the empty joeyProfile friends collection.
    
* [ ] Loop through the allUsers array.  
     On each iteration, we'll have a single user object. 
    
* [ ] If a user in the allUsers array is from the same city as joeyProfile,  
     push the username to the joeyProfile friends array.

3) Next, let's add some coworkers to the empty joeyProfile coworkers collection.
  
* [ ] Loop through the allUsers array.
  
* [ ] If a user in the allUsers array has the same job as Joey,  
   push the username to the joeyProfile coworker array.

4) Next, let's add some family members to the empty joeyProfile family collection.
  
* [ ] Loop through the allUsers array.
  
* [ ] If a user in the allUsers array has the same last name,  
   push the username into the joeyProfile family array.
  
* [ ] **You'll have to do something special to check JUST the last name.  
   Check out the split() function.**

5) Now let's make sure there aren't any duplicate usernames in our friends and family arrays.  
   *  If 'Doug Flutie' is in our family array, it shouldn't be in our friends array.  
   *  If it is, let's delete it from our friends array, as family is more important to Joey.
   
* [ ] Loop through our family array.
   
* [ ] Inside of our family loop, loop through our friends array.  
   What this is doing?  
   As we loop through each family member,  
   check that family member against every person in the friends array.  
   
* [ ] If the current family member is equal to the current element of our friends array,  
   delete that element from our friends array.
   
* [ ] There are a couple of ways to delete things from an array.  
   Look up .splice() and try to use that.

6) Now let's make sure there aren't any duplicate usernames in our friends and coworkers arrays.  
   *  If 'Doug Flutie' is in our friends array, it shouldn't be in our coworkers array.  
   *  If it is, let's delete it from our coworkers array, as friends are more important to Joey.
   
* [ ] Loop through our friends array.
   
* [ ] Inside of our friends loop, loop through our coworkers array.
   
* [ ] If the value of the current element inside of our coworkers array is equal to  
   the current element of our friends array, delete that element from our coworkers array.

    ### YOU ARE NOW ENTERING HARD MODE (EXTRA CREDIT)

7) Now that we have all of our arrays filled, let's sort each array by alphabetical order.

* [ ] Create a function called nameSort that takes an array and sorts its contents by alphabetical order.  
   **hint: arrays may have a method that does this.**

* [ ] Use nameSort on each array in our joeyProfile object.

* [ ] Check each array by using console.dir to make sure its contents are sorted by the end.

8) Joey wants to be able to instantly look up whether someone is in one of his networks.

* [ ] Create a function, networkCheck, that takes an array and a name.

* [ ] If the name exists in the array, alert() the users full profile formatted exactly like the example below.

     ```
    nameCheck(friendsArray, 'Solomon Daniels');

    'Name: Solomon Daniels
    Job: Engineer
    City: Berkeley, California
    Friends: 0,
    Family: 0,
    Coworkers: 0'
    ```
* [ ] If the person doesn't exist,
   * [ ] set up a prompt that  
   * [ ]  asks for the friend's info (name, job, city), and  
   * [ ]  adds it to an object named newUser.  
   (newUser should also have friends, family, and coworkers arrays inside of it -- sound familiar?).

* [ ] Add newUser's name to the input array passed to nameCheck.  
   Call nameCheck on the array to make sure it exists.
   
* [ ] Add newUser object to the array `allUsers`.
     console.dir the allUsers variable and see if the newUser you added exists.
