# vaccine-management-system
## problem statement
  C++ Program to manage the roll out of Covid-19 vaccine where an eligible user can
  register for his vaccine dose, be allotted his timeslot, take the vaccine, and leave after he/she is done.
## Some of the important functions of our code are as follows:
### 1. registration():
The user is prompted to enter his personal details. 
Here we check if the user is eligible for the vaccination depending upon his age. 
If he is eligible, the user is passed onto the enqueue function.
### 2. admin_login():
Admin is prompted to enter his password and upon authentication has access to 
various functionalities of the Admin Class. 
He can set an available_slots variable depending on the vaccines that the vaccination center 
is going to receive and also change the age eligibility for the vaccination depending on 
the government guidelines. 
The most important functionality of the Admin class is run_process().
### 3. run_process():
Using the ctime library, we have calculated the date on which the process is being run.
Citizens are allotted slots only for the next day. 
This function makes use of helper functions from the dateutil header files to calculate the next date.
### 4.user_login():
This function enables the user to login and check his allotted time slot. 
He is expected to log in on the day of his vaccination and confirm his vaccination. 
Upon being vaccinated he is dequeued. 
If a user fails to do so, he is demoted to the end of the queue and his priority decremented. 
This process is implemented with the help of dequeue() and remove() functions respectively.
### 5.Extra:
Other functionalities of the Admin and the Citizen class are looking up the list of citizens who are  
supposed to get vaccinated today and looking up the top 'n' entries from the vaccination queue.
