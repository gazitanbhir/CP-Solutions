# CP-Solutions



Joy and Bijoy are two friends who participated in GSF Hacks Prelims on WUB, and both of them easily qualified for the on-site round. Joy wants to team up with Bijoy for the on-site round but Bijoy has a date with his girlfriend the same day. Joy thus plans to spoil Bijoy’s date and trigger their breakup.

Bijoy and his girlfriend both use a chat application developed by Joy. Joy can read all the messages sent using his app, so he first wants to know whether they have postponed or preponed their date or not. To confirm the same Joy has decided to search for all the days they have discussed in the past week and see which of the day is decided for the date. GSF Hacks is on 19th and 20th, if they are going on a date on some other day Joy can attend GSF Hacks with his friend, otherwise he will have to come up with some other idea. Joy knows that when his friend and his [friend’s] girlfriend have to choose a day, the girlfriend's choice is given twice more weightage than Bijoy's.

The problem is that Bijoy and his girlfriend talk a lot (-_-) and have a very long chat history which Joy cannot read manually to know about their date. Joy asks you to help him write a program that can do the same.

He provides you with the chat history in following format.

[G/M]*: <message>   
 G: I want to go on 19  
 M: No that is not possible lets go on 21  
 G: No 19 is final and 21 is not  
 M: OKAY as you wish

*[G means that it is Girlfriend’s message and M means that it is Menot’s message]

In the above chat history we can see that 19 have been discussed twice and 21 has also been discussed twice. But 19 have weightage 4 and 21 has weightage 3. Disregard human logic, "21 is not" will still add 21 to the weightage -- you do not need to implement NLP. Joy thus knows that 19 has been finalised.

Note: If multiple days have same MAXIMUM weightage the date is cancelled.

Input:
First line contains an integer N and then N lines follow with a message S in the following format in each line.
[G/M]:
eg. G: Hi
[G means that it is Girlfriends message and M means that it is Menot’s message]
Note: Everything is space separated and the days will be integers with no leading zeroes and will always be preceded by a space]

Output : Print “Date” if the decided day is 19 or 20 otherwise print “No Date”.
Note: If multiple days have same weightage the date is cancelled and you must output “No Date”

Constrains
1 <= N <= 1000
2 <= |S| <= 1000 [ Length of each message ]
1 <= Day <= 30 [ Days discussed in the chat ]
SAMPLE INPUT
 

4
G: I want to go on 19
M: No that is not possible lets go on 21
G: No 19 is final and 21 is not
M: OKAY as you wish

SAMPLE OUTPUT

Date

File submissions 
