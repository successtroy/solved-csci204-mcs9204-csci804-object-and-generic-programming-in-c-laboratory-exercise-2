Download Link: https://assignmentchef.com/product/solved-csci204-mcs9204-csci804-object-and-generic-programming-in-c-laboratory-exercise-2
<br>
<strong>Task 1: Basic class/object construction (1.0) </strong>

A basketball union manage the competitions among the teams. There is a text file contains results of the competitions. The format for each competition is like

team1-name:team2-name score1:score2




Define a class <strong>Team</strong> in the file <strong>competition.h</strong> that contains a team name, total win, total loss, total score for, total score against. Define the necessary member functions for the class, such as default constructor and other member functions to set and get data members’ values.

Define a class <strong>Result</strong> in the file <strong>competition.h</strong> that contains an array of <strong>Team</strong> with maximum 10 elements, an integer number counts how many teams. Define the following member functions for the class.

<ul>

 <li>A load function that loads competition results from a given text file, analysis each competition result by modify the two teams’ information as following:</li>

</ul>

o If a team is not exists in the Team array, add the team in the Team array. o If the team already exists, modify the team’s data by

Increase the total win by one if the team won the competition;

Increase the total loss by one if the team lost;

Add the score that the team has got to the total score for;

Add the score that opponent team has got to the total score against.

<ul>

 <li>A sort function that sorts the teams in the descending order according to the total win. If the total win times are the same, compare the total loss time, the less the better. If the total win and total loss times are the same, compare the differences of total score for and total score against, the bigger the better. The sorting algorithm is up to you.</li>

 <li>A print function print out the teams’ records to screen.</li>

</ul>

Implement the member functions in a file <strong>competition.cpp</strong>.

Write C++ driver program include main function in a file <strong>basketball.cpp</strong> that read a file name of competition results from keyboard, declare an instance of Result, load the competition results by using the instance of <strong>Result</strong>, analyse the results, sort the records and print out all teams’ information in the descending order.

You can download a file <strong>results.txt</strong> from the site for your testing. The example output results will be like:

Input a basketball competition results’ file name: results.txt

<table width="348">

 <tbody>

  <tr>

   <td width="240">Shellharbour                           10</td>

   <td width="48">0</td>

   <td width="60">471  100</td>

  </tr>

  <tr>

   <td width="240">Raptors                                    6</td>

   <td width="48">5</td>

   <td width="60">227  257</td>

  </tr>

  <tr>

   <td width="240">Bobcats                                   6</td>

   <td width="48">5</td>

   <td width="60">178  225</td>

  </tr>

  <tr>

   <td width="240">Spurs                                       6</td>

   <td width="48">6</td>

   <td width="60">275  270</td>

  </tr>

  <tr>

   <td width="240">MTSO Warriors                      5</td>

   <td width="48">7</td>

   <td width="60">234  273</td>

  </tr>

  <tr>

   <td width="240">Mavericks                               1</td>

   <td width="48">11</td>

   <td width="60">159  419</td>

  </tr>

 </tbody>

</table>





