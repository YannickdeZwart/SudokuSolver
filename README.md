# SudokuSolver

this project uses a algoritme to solve a sudoku

what the algoritme does is it searches a every square untill it finds a 0


        {7, 0, 2, 0, 5, 0, 6, 0, 0}
        {0, 0, 0, 0, 0, 3, 0, 0, 0}
        {1, 0, 0, 0, 0, 9, 5, 0, 0}
        {8, 0, 0, 0, 0, 0, 0, 9, 0}
        {0, 4, 3, 0, 0, 0, 7, 5, 0}
        {0, 9, 0, 0, 0, 0, 0, 0, 8}
        {0, 0, 9, 7, 0, 0, 0, 0, 5}
        {0, 0, 0, 2, 0, 0, 0, 0, 0}
        {0, 0, 7, 0, 4, 0, 2, 0, 3} 

when it finds the 0 it loops trough the number 1 to 9 untill it finds a number that can go on the spot. when it finds it it fills it in and loops again.

when it can't find any numbers that can go in the spot it will revert the previous number and search for a number again. then it loops back to the previous number.

When its done it outputs this:

    Solved successfully!
    732|458|619
    956|173|824
    184|629|537
    -----------
    871|564|392
    643|892|751
    295|317|468
    -----------
    329|786|145
    418|235|976
    567|941|283
    
In this example the board is unsolveable because there are 2 7's in a row:

    Unsolvable board :(
    702|050|670
    000|003|000
    100|009|500
    -----------
    800|000|090
    043|000|750
    090|000|008
    -----------
    009|700|005
    000|200|000
    007|040|203
    
    
    
Some other examples:

Hardest sudoku in the world
Input:

    {8, 0, 0, 0, 0, 0, 0, 0, 0}
    {0, 0, 3, 6, 0, 0, 0, 0, 0}
    {0, 7, 0, 0, 9, 0, 2, 0, 0}
    {0, 5, 0, 0, 0, 7, 0, 0, 0}
    {0, 0, 0, 0, 4, 5, 7, 0, 0)
    {0, 0, 0, 1, 0, 0, 0, 3, 0}
    {0, 0, 1, 0, 0, 0, 0, 6, 8}
    {0, 0, 8, 5, 0, 0, 0, 1, 0}
    {0, 9, 0, 0, 0, 0, 4, 0, 0}

Output: 

    Solved successfully!
    812|753|649
    943|682|175
    675|491|283
    -----------
    154|237|896
    369|845|721
    287|169|534
    -----------
    521|974|368
    438|526|917
    796|318|452

Input:

    {0, 3, 0, 4, 0, 9, 5, 1, 0}
    {0, 0, 0, 7, 0, 3, 4, 0, 0}
    {8, 9, 4, 2, 0, 0, 6, 0, 3}
    {9, 8, 0, 0, 0, 0, 0, 0, 0}
    {0, 0, 0, 0, 0, 0, 0, 0, 7}
    {0, 0, 6, 3, 0, 2, 0, 0, 1}
    {2, 0, 3, 8, 0, 0, 0, 0, 0}
    {0, 7, 0, 9, 3, 0, 0, 6, 0}
    {1, 0, 9, 0, 2, 4, 0, 0, 0}

Output:

    Solved successfully!
    637|489|512
    512|763|489
    894|215|673
    -----------
    985|147|326
    321|658|947
    746|392|851
    -----------
    253|876|194
    478|931|265
    169|524|738

Input:

    {0, 0, 0, 0, 0, 9, 0, 4, 7)
    {0, 0, 9, 0, 0, 7, 8, 0, 0}
    {4, 3, 0, 8, 5, 2, 0, 0, 0}
    {9, 0, 0, 0, 0, 0, 0, 5, 1}
    {0, 0, 4, 0, 0, 0, 7, 0, 0}
    {6, 1, 0, 0, 0, 0, 0, 0, 4}
    {0, 0, 0, 9, 2, 4, 0, 7, 8}
    {0, 0, 2, 5, 0, 0, 1, 0, 0}
    {7, 9, 0, 1, 0, 0, 0, 0, 0}

Output:

    Solved successfully!
    586|319|247
    129|467|835
    437|852|916
    -----------
    973|248|651
    254|631|789
    618|795|324
    -----------
    361|924|578
    842|576|193
    795|183|462
 
