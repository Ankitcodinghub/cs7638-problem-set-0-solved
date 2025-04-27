# cs7638-problem-set-0-solved
**TO GET THIS SOLUTION VISIT:** [CS7638 Problem Set 0 Solved](https://www.ankitcodinghub.com/product/cs-7638-roboticsai-techniques-problem-set-0-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;123483&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS7638  Problem Set 0 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
[Note that PS0 does not count towards your grade.]

Introduction

This is a problem set to introduce some basic Python features, ensure your environment is correctly set up, and practice submitting to Gradescope. It is ungraded, but you should still complete it.

Working with Python

All the questions have you write methods in Python classes. Please refer to https://docs.python.org/3/tutorial/classes.html for a refresher on classes in Python if required. You are required to make changes to ps0_answers.py, and you can test if your solution is working correctly by running the same locally.

You will need to have set up your Python interpreter and class environment to complete this problem set, so refer to the Environment Setup pdf for guidance.

Question 1

Consider a bank account which provides three operations:

1. deposit to add an amount parametrized by a non-negative integer amount.

2. withdraw to withdraw an amount parametrized by a non-negative integer amount. You can be assured that amount will never be greater than the balance at any time, so you need not worry about that scenario.

3. getBalance to fetch the balance at any given time.

The bank account starts with a zero balance, so you can initialize the balance as zero in the __init__ method.

You need to edit the class Question1 in file ps0_answers.py for this quiz. Gradescope (our autograder) will invoke the above three methods repetitively in some fashion to ensure that the implementation is correct. As an example, the below sequence of lines should run without an error.

account1 = ps0_answers.Question1() assert account1.getBalance() == 0 account1.deposit(100) account1.deposit(20)

assert account1.getBalance() == 120 account1.withdraw(50) assert account1.getBalance() == 70 account1.deposit(20) assert account1.getBalance() == 90

The file ps0_answers.py includes test cases that can be run from the command line.

Question 2

This time we are maintaining the number of dimes and quarters instead of the balance. There are the following operations available:

1. __init__: initialization of the number of dimes and quarters.

2. addCoins: to add dimes and quarters as specified in the parameter dictionary dimes_and_quarters.

3. removeCoins: to remove dimes and quarters as specified in the parameter dictionary dimes_and_quarters.

4. getCoins: returns the number of dimes and quarters we have after additions and removals in a dictionary.

1

5. getBalanceCents: returns the balance from the remaining dimes and quarters.

An example of sequence of the methods that should run without an error is:

account2 = ps0_answers.Question2({‘dimes’: 5}) account2.addCoins({‘dimes’: 2, ‘quarters’: 10}) assert account2.getBalanceCents() == 320

assert account2.getCoins() == {‘dimes’: 7, ‘quarters’: 10} account2.removeCoins({‘dimes’: 2, ‘quarters’: 10}) assert account2.getCoins() == {‘dimes’: 5, ‘quarters’: 0} assert account2.getBalanceCents() == 50

Question 3

This question is almost same as question 2, except that the input parameter type for addCoins and removeCoins methods is a tuple instead of dictionary. There are the following operations available:

1. __init__: initialization of the number of dimes and quarters.

2. addCoins: to add dimes and quarters as specified in the parameter tuple dimes_and_quarters.

3. removeCoins: to remove dimes and quarters as specified in the parameter tuple dimes_and_quarters.

4. getBalanceCents: returns the balance from the remaining dimes and quarters.

Please refer to the docstring of the respective methods of class Question3 in ps0_answers.py for more details. An example sequence of the methods that should run without an error is:

account3 = ps0_answers.Question3({‘dimes’: 5}) account3.addCoins((2, 10)) assert account3.getBalanceCents() == 320 account3.removeCoins((2, 10)) assert account3.getBalanceCents() == 50

Question 4

It is common to make mistakes while coding, and a traceback of the error is the most helpful thing in debugging errors. This question already has all the code implemented, but there is an error when we execute it. The task in this quiz is to get rid of the error and get back the intended value.

There are two methods that this quiz provides: 1. __init__ which initializes the accounts of different customers. 2. displayBalance which returns a string to display the balance for all the customers.

An example of a sequence of lines that will be executed in Gradescope and that should run without error is: account4 = ps0_answers.Question4({ ‘Alex’: (5, 10), ‘Bob’: (0, 2) }) assert quiz4.displayBalance() == ‘(Customer: Alex, Balance: 300)(Customer: Bob, Balance: 50)’

Testing

There are several test cases provided. Make the required changes to ps0_answers.py and you can run this file locally to test before submitting. The final score is out of 100.

Submission

Make the required changes to the file ps0_answers.py and submit to Gradescope once complete.

2
