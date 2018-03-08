# Calculate the mirror of binary tree.
         8
       6   10
      5 7 9 11
        to 
         8
       10  6
      11 9 5 7   
        
pre-order iterate, trasfer tree if not null
          8
        6   10
       5 7 9 11
           8
        10   6
       9 11 5 7
           8
        10   6
       11 9 5 7
           8
        10   6
       11 9 5 7