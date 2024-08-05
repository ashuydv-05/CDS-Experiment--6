# CDS-Experiment--6
## Aim:To study and implement C++ decision making statements Loops
## Theory:
In C++, loops are necessary to run a code block repeatedly. When the number of iterations is known ahead of time, the for loop is utilized. It is composed of an increment/decrement statement, a condition, and an initialization. When the number of iterations isn't preset, the while`loop is handy because it keeps running as long as its condition holds true. Similar to the while loop, the do-while loop ensures that the code block executes at least once prior to the condition being tested. Loops improve program functionality by handling repeating activities efficiently and minimizing the need for unnecessary code. Using loops correctly is essential to developing efficient and well-designed C++ programs.
## Code:
```

//Ashu Yadav
//23070123154

#include <iostream>
using namespace std; 

int main()
{
    //do-while
    cout<<"Using do while loop: "<<endl;
    int a = 10;
    do
    {
        cout<<a<<endl;
        a--;
    } while (a != 0);

    cout<<endl;
    cout<<endl;

   //for loop
    cout<<"Using for loop: "<<endl;
    int i = 0;
    for(i = 0; i <=10;i++)
    {
        cout<<i<<endl;
    }
    cout<<endl;
    cout<<endl;

    //while loop
    cout<<"Using while: "<<endl;
    int b = 10;
    while(b>0)
    {
        cout<<b<<endl;
        b--;
    }
    cout<<endl;
    cout<<endl;

    //for loop
    cout<<"Using for: "<<endl;
    for(i = 0; i <=100; i = i + 5 )
    {
         cout<<i<<endl;
    }
    cout<<endl;
    cout<<endl;

    //nested for - pattern
    cout<<"Using nested for loops for pattern: "<<endl;
    int ii,j,k = 0,n2 = 5;
    for(ii = 1; ii <= n2; ii++)
    {
        for(j = 1; j <= (n2-ii);j++)
        {
            cout<<" ";
            while(k != (2*ii-1))
            {
                cout<<"* ";
                k++;
            }
            k=0;
            cout<<endl;    
        }   
        cout<<endl;
    }
    cout<<endl;
    cout<<endl;

    //nested do while
    cout<<"Using nested do-while to find the product of numbers:"<<endl;
    int q = 0,r = 0;
    do
    {
        q++;
        do
        {
            r++;
            cout<<"Product of two numbers:  "<<q*r<<endl;
        }while(r<10);
        

    } while(q<10);
    cout<<endl;
    cout<<endl; 

    //nested while
    cout<<"Sum of 2 numbers using nested while: "<<endl;
    int q2 = 10, r2 = 10;
    while(q2>0)
    {
        q2--;
        while(r2>0)
        {
            r2--;
            cout<<"Sum: "<<q2+r2<<endl;
        }

    }
    cout<<endl;
    cout<<endl; 
    
    //nested for - matrix
    cout<<"Using nested for loops for matrix: "<<endl;
    int m,n,p;
    int mat[2][2][2] = {
                            {
                                {1, 2},
                                {3, 4}
                            }, 
                            {
                                {5, 6}, 
                                {7, 8}
                            }
                        };

    for (int m = 0; m < 2; ++m) 
    {
        for (int n = 0; n < 2; ++n) 
        {
            for (int p = 0; p < 2; ++p) 
            {
                cout<<mat[m][n][p];
            }
            cout<<endl;
        }
    }
    cout<<endl;
    cout<<endl; 
    
    //nested for + while - matrix
    cout<<"Using nested for loops and while for matrix and checking some condition: "<<endl;
        int m1,n1,p1;
        int mat1[2][2][2] = {
                                {
                                    {1, 2},
                                    {3, 4}
                                }, 
                                {
                                    {5, 6}, 
                                    {7, 8}
                                }
                            };

        for (int m1 = 0; m1 < 2; ++m1) 
        {
            for (int n1 = 0; n1 < 2; ++n1) 
            {
                for (int p1 = 0; p1 < 2; ++p1) 
                {
                    while(mat1[m1][n1][p1] < 8)
                    {
                        cout<<mat1[m1][n1][p1];
                        break;

                    }
                    
                }
                cout<<endl;
            }
        }
    cout<<endl;
    cout<<endl; 

   return 0;
}
```
## Output:
![exp](https://github.com/ashuydv-05/CDS-Experiment--6/blob/main/6a.png)
![exp](
![exp](
![exp](

## Conclusion:
We learnt about loops and their use case.
