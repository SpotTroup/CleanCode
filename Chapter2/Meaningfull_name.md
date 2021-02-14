# Chapter 2:  Meaningfull name
We use lots of naming in our code like variable name, class name , function name etc. Clean code requires clean and meeningfull names. 
There are some simple rules for good naming in code.
 ## Use Intention-Revealing Names
 Every name in your code have to have a name that describe its use and perpose. You also can leave a comment for description .
 For example we have piece of code here.
 ```
 public List<int[]> getThem() {
List<int[]> list1 = new ArrayList<int[]>();
for (int[] x : theList)
if (x[0] == 4)
list1.add(x);
return list1;
}
 ```
 
 Here   getThem ,List1 , the list ,x[0]  blah blah means nothing. You are the author and your writing is quite meaningless , smile.
 What is list1?
 why there is 4?
 what do you mean by them?
 There is no answer in those codes. So every name must reavile what do you intet to.
 Suppos this is a boardgame code with which we will get the flagged cells.
  ```
  public List<int[]> getFlaggedCells() {
List<int[]> flaggedCells = new ArrayList<int[]>();
for (int[] cell : gameBoard)
if (cell[STATUS_VALUE] == FLAGGED)
flaggedCells.add(cell);
return flaggedCells;
}
  
  ```
  Notice carefully the code doesnt get more complex or large , it is still the same but more meaningfull.
   ## Avoid Disinformation
   Dont place any name that far from intended meaning. Like hp, eco, aix those are poor variable name to give , those have special meaning programming. 
   Another thing is group , list or bunch. If you say numberlist it will like list variable . So could be groupOfNumber or bunchOf Number.
   A truly disinformative name is with lower case of l and uppercase of o. Like
     ```
     int a = l;
if ( O == l )
a = O1;
else
l = 01;
       ```
   Too much congusing about 0 or O and 1 or l
   
   ## Make Meaningful Distinctions
When you want to declare some series variable dont do this like a1[] , a[]2.... Those are not disinformative those noninformative. Not a clue what are going to do with this.
Noise words are another meaningless distinction. Supppose you have Car class , then you have added CarDetails or CarInfo. Those are with same meaning with different class.
Another thing should must avoid that redudndant naming. Like NameString , CarObject , VarCar . Name will be always string for coding sake. And keep giving var in variable name is like giving name human to a human.
## Use Good Names
Good names means pronouciable and searchable names. That is easier to understand . Again you are a author and you have to make others to understand. That people can understand this name and its work . On the otherhand people can search easily your varibles by its use. 
It is good practice to use more short name in local variable that global variable.
 ## Always Avoid Encoding
 We tend to give name as short form. Like phonNum, AddInfo(Address info). It is too much confusing and another burden.  In modern IDE we dont need to do this . If you give complete name  ,it will enforce you write the full name. 
 Another problem in namig is prefix . like m_somethinf , f_something. We dont those. For example 
  ```
 public class Part {
private String m_dsc; // The textual description
void setName(String name) {
m_dsc = name;
}
}
_________________________________________________
public class Part {
String description;
void setDescription(String description) {
this.description = description;
}
}
 ```
 
 ## Some tips for Class and Method Names
 ### Class
 * Class name shoud be Noun or none phrase like employee , Customer. 
 * Avoid data, info ,item in those name.
 ### Function
 * Function name should be verb or verb phrase. Like getCustomers , addEmployee.
 * Always try to add some prefix like get,add , post etc.