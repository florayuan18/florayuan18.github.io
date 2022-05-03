---
layout: page
title: Study Week 2
subtitle: Flora Yuan
---
## Study Week 2
Requirements
* MCQ results
* ![studyweek2.png](/assets/img/studyweek2.png)
* MCQ Test Corrections:
Q1:
int a = 3 + 2 * 3;

int b = 4 + 3 / 2;

int c = 7 % 4 + 3;

double d = a + b + c;

* I think I rushed on this question because I was concerned about time.  The answer should be 20.0, but I chose 20.5 because I thought it's a floating point division rather than an integer division with int b = 4 + 3.0/2.  The correct answer was actually 20.0, where the multiplication operation is evaluated before the addition operation.

Q2:
if (num > 0)
{
    if (num % 2 == 0)
    {
        System.out.println("A");
    }
    else
    {
        System.out.println("B");
    }
}

* The only thing I mixed up in this question was the odd vs even integers. I mixed up num % 2 == 0 to be num % 2 != 0.

Q4:
public static void message(int a, int b, int c)
{
    if (a < 10)
    {
        if (b < 10)
        {
        System.out.print("X");
        }
        System.out.print("Y");
    }
    if (c < 10)
    {
        if (b > 10)
        {
            System.out.print("Y");
        }
        else
        {
            System.out.print("Z");
        }
    }
}

* Here, I missed an extra Y in the final printed result.  I looked at the result if the call message was 15,15,5 instead of 5, 15, 5.  I think this was also as a result of thinking I needed to work very fast in the beginning of the test.

Q5:
public class Bird
{
    private String species;
    private String color;
    private boolean canFly;
    public Bird(String str, String col, boolean cf)
    {
        species = str;
        color = col;
        canFly = cf;
    }
}

* This was also a silly mistake.  I didn't double check that the constructor's sginature was the same from the original constructor, and I only looked at the content in the middle of the brackets.

Q19:
int[][] values = {{1, 2, 3}, {4, 5, 6}};
int x = 0;
for (int j = 0; j < values.length; j++)
{
    for (int k = 0; k < values[0].length; k++)
    {
        if (k == 0)
        {
            values[j][k] *= 2;
        }
        x += values[j][k];
    }
}

* I forgot that I needed to double the first element of each row.  The correct answer should include this factor, so it would be 2 + 2 + 3 + 8 + 5 + 6 = 26.  I would need to review the details/rules of arrays again by watching the faculty lecture.

Q21:
String[] testOne = {"first", "day", "of", "spring"};
String[] resultOne = strArrMethod(testOne);

* I misread the code.  I thought that it would be necessary to organize based on string length, with the smallest strings coming first.  However, it seems like of, of, of, spring is the right answer because the method assigns the shortest string between arr[0] and arr[3].  Since the shortest string appears again, of would be repeated two more times.

Reflection: I think that for taking the test with no studying, I did pretty okay.  I think that I have a good amount of the basic concepts, but I need to brush up on other concepts.  I think my next steps moving forward would just be to watch more of the university lectures and applying the knowledge to the PBL projects.
* I had to guess on the last 10 questions, so I will add in more revisions for next week.

* FRQ results (didn't do/not taking the test)
* Effort/Ticket/GH Pages

## PBL Focus + Reflection
* PBL --> We kind of talked about this in class, but I think everyone in the group is a bit confused on how to move forward with the project.  The PBL tidbits we're taking on don't seem to be super clear, so we are thinking of restructuring the project as a whole.  FOr now, I worked on creating some sort of login page for the website.
* [some pbl before switch](https://github.com/adhithin/lab-kit/commit/3666b7a40c17dcb732c25800c72c07fc4116e814)
* Some starting code for a potential login page.  Will be working on the database aspect of the login page afterwards
* Reflection Compared to Last Trimester: Last trimester the login page that I coded did not have the full capabilities that were necessary.  It displayed the information unique to each user, but I wasn't able to figure out how to make a specific register page to add in new users (used arrays instead).  This is an issue I want to fix for this project.

## Participation
* Here for class Monday - Thursday