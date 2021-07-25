## Class 02
## Packages and Import
the package is the container of many files (classes) , and it should be the same name with the name of the folder that contain the classes 
and we can use another packages from another library using the import statement

**the package deceleration should be the first statement inside the java file**

## three options to import 
- import javax.swing.*;  // Make all classes visible altho only one is used.
- import javax.swing.JOptionPane;  // Make a single class visible.
- javax.swing.JOptionPane.showMessageDialog(null, "Hi"); //without import

## the types of loops that we can find in Java:
- Simple for loop
          
            for (int i = 0; i < 5; i++) {
                System.out.println("Simple for loop: i = " + i);
            }
- Enhanced for-each loop

            for(Type item : items)
            statement;
- While loop

            while (Boolean-expression) 
            statement;
- Do-While loop

            do {
            statement;
            } while (Boolean-expression);

