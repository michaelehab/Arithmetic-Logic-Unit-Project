# Arithmetic-Logic-Unit-Project
In this project, we designed and implemented an arithmetic unit that is capable of adding, subtracting and multiplying two signed numbers, and displays the result of the operation performed along with some additional flags regarding the operation and the result.

![Diagram](https://github.com/michaelehab/Arithmetic-Logic-Unit-Project/blob/main/img/project.jpg)
## Description
<ol>
  <li>
    Reminder: Result = A % B
    <p>During the division A, B and Result are 3-bits signed numbers.
A % 0 is forbidden and must output 0 and Div by Zero Flag must be asserted
A % B, has the same sign as A.</p>
For example: +2%+3 =+2, +2%-3 =+2, -2%+3=-2, -2%-3=-2
    </p>
  </li>
  
  ![Remainder Circuit](https://github.com/michaelehab/Arithmetic-Logic-Unit-Project/blob/main/img/remainder.jpg)
  <li>
    Multiplication: C = A * B
    <p>During the multiplication, A and B are 3-bits signed numbers and C is a 5-bits signed number. The
multiplication of 2-bits by 2-bits yields a result of 4-bits, therefore is composed of 4-bits for the
value and 1-bit for the sign.</p>
For example: +2%+3 =+2, +2%-3 =+2, -2%+3=-2, -2%-3=-2
  </p>
  </li>
  
  ![Multiplication Circuit](https://github.com/michaelehab/Arithmetic-Logic-Unit-Project/blob/main/img/multiplication.jpg)
  <li>
    Addition: C = A + B
    <p>During the addition, A, B, and C are all 3-bits signed numbers.
      </p>
  </li>
  <li>
    Subtraction: C = A - B
    <p>During the subtraction, A, B and C are all 3-bits signed numbers.
      </p>
  </li>
  
![Two's Complement Circuit](https://github.com/michaelehab/Arithmetic-Logic-Unit-Project/blob/main/img/twoscomplement.jpg)
![Adder/Subtractor Circuit](https://github.com/michaelehab/Arithmetic-Logic-Unit-Project/blob/main/img/addersubtractor.jpg)
</ol>

## Flags
<ul>
  <li>
    Sign Flag:
    <p>The sign flag indicates if the result is negative. The flag is set to 1 if the result is negative and 0 otherwise.</p>
  </li>
  <li>
    Zero Flag:
    <p>The zero flag indicates if the result is zero. The flag is set to 1 if the result is zero and 0 otherwise.</p>
  </li>
  <li>
    Div by Zero Flag:
    <p>The divide by zero flag indicates if we divide by zero. The flag is set to 1 if B operand equal zero in division operation and 0 otherwise.</p>
  </li>
</ul>

## Integration Circuit

![Integration Circuit](https://github.com/michaelehab/Arithmetic-Logic-Unit-Project/blob/main/img/integration.jpg)

Note : We used the <a href="https://github.com/marceloboeira/logisim-7-segment-display-driver">logisim-7-segment-display-driver by marceloboeira</a>
