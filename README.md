# Binary-Search-Algorithm
A Binary Search Algorithm basically searches for an element in a list or array 
'''Considering the list below'''
2  4  6  8  10  12  14  16  18  20 
'''Setting pointers that reflect the highest and lowest value in the list'''

#lets define a function for the binary search


  defFindElement(elements,elementToFind):

     low=0
     high=len(elements)-1

    while low<=high:
  
      mid=low+(high+low)//2

      if elements[mid]== elementToFind:
        return mid

      elif elementToFind>elements[mid]:
        low=mid+1

      else:
        high=mid-1
    return-1

#adding the following code to the program, outside the _FindElement_ function

    elements = [2,4,6,8,10,12,14,16,18,20]
    elementToFind = 12

    final = FindElement(elements, elementToFind)

    if final == -1:
      print("This item was not found in the list")
  
    else:
      print("The number" + str(elementToFind) + "was found at index position" + str(final) + ".")
  
  
