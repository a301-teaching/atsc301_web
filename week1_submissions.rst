.. _submissions:

Some submission examples
------------------------

C++
+++

.. code-block:: c++
    
    #include <iostream>
    #include <fstream>
    #include <string>
    
    using namespace std;
    
    int main() {
            
            string line; // the line read from input.txt
    
            ifstream myfile; //opens stream for reading files
    
            myfile.open ("input.txt"); //opens input.txt for reading in myfile stream
    
            if (myfile.is_open()) 
            {
                    getline(myfile,line);   //assigns line the only line from input.txt
            }
            else cout << "Unable to open file";
    
            size_t delimiter = line.find(";"); // assigns  the character ";" as the delimiter of 
                                                                               // unsigned integral type size_t
    
            string tc = line.substr(0,delimiter);   // gets first part of line before delim, the total count
            string ss = line.substr(delimiter + 1); // gets second part after delim, the step size
    
            //cout << tc << " " << ss ;
    
            int total_count = atoi(tc.c_str());
            int step_size = atoi(ss.c_str());
    
            //cout << total_count << endl;
            //cout << step_size << endl;
    
            for (int i=total_count; i>0; i+=step_size )
                    cout << i << endl;
    
            myfile.close();
            return 0;
    }
    

Python
++++++

.. code-block:: python

    """
    
    week1.py
    ATSC 301
    
    Reads from a text file, input.txt, and takes in the two 
    integers. Loops from the first integer down to zero with
    a step size equal to the second integer, printing out
    the loop integers along the way.
    
    """
    
    # open and read from input.txt in cwd
    
    with open('input.txt','r') as file1:
        line = file1.read()
    
    # separate line into two distinct strings, using ; as the delimiter
    numbers = line.split(';')
    
    # extract the strings from the array and convert both to integers
    # set first integer to be the starting number 
    # set second integer to be the step size 
    total_count = int(numbers[0])
    step_size = int(numbers[1])
    
    # main loop; print out the loop integers all the way down to 0
    for i in range(total_count,0,step_size):
        print i

Java
++++

.. code-block:: java

    import java.io.IOException;
    import java.io.FileReader;
    import java.io.BufferedReader;
    
    public class Steps {
    
            public static void main(String[] args) throws IOException {
                    FileReader fr = new FileReader("input.txt");
                    BufferedReader textReader = new BufferedReader(fr);
                    String textData = textReader.readLine();
                    String firstNum = "";
                    String secondNum = "";
                    
                    int position = textData.indexOf(";");
                    firstNum = textData.substring(0, position);
                    secondNum = textData.substring(position + 1, textData.length());
                    
                    int total_count = Integer.parseInt(firstNum);
                    int step_size = Integer.parseInt(secondNum);
                    System.out.println("The initial count is " + total_count + ".");
                    
                    int count = 1;
                    while (total_count > 0) {
                            
                            total_count = total_count + step_size;
                            System.out.println("The total count is " + total_count + ".");
                            System.out.println("The loop has executed " + count + " times.");
                            count++;
                    }
                    
            }
    }


Matlab
++++++

.. code-block:: matlab

    clc
    clear
    
    M = dlmread('input.txt', ';');
    count = M(1);
    step = M(2);
    array = count:step:0;
    disp(array);
