# LetsUpgrade-AI-ML-
LetsUpgrade AI/ML 
%%html
<style>
body{
    font-family:"Comic Sans MS",cursive,sans-serif;
}
</style>
1:
Assuming that we have some email addresses in the "username@companyname.com" format, please write program to print the company name of a given email address. Both user names and company names are composed of letters only. Input Format: The first line of the input contains an email address. Output Format: Print the company name in single line. Example; Input: john@google.com Output: google

ip=input()
x=ip.index("@")
print(ip[x+1:len(ip)-4],end='')
nikhil@sohum.com
sohum
 
2: Write a program that accepts a comma-separated sequence of words as input and prints the words in a comma
separated sequence after sorting them alphabetically. Input Format: The first line of input contains words separated by the comma. Output Format: Print the sorted words separated by the comma. Example: Input: without,hello,bag,world Output: bag,hello,without,world

items = input("Input comma separated sequence of words")
words = [word for word in items.split(",")]
print(",".join(sorted(list(set(words)))))
Input comma separated sequence of wordswithout,hello,bag,world
bag,hello,without,world
 
4: Given a list of n-1 numbers ranging from 1 to n, your task is to find the missing number. There are no duplicates.
Input Format: The first line contains n-1 numbers with each number separated by a space. Output Format: Print the missing number Example: Input:1 2 4 6 3 7 8 Output:5 Explanation: In the above list of numbers 5 is missing and hence 5 is the input

def getMissingNo(A): 
    n = len(A) 
    total = (n + 1)*(n + 2)/2
    sum_of_A = sum(A) 
    return total - sum_of_A 

A = [1, 2, 4, 5, 6] 
miss = getMissingNo(A) 
print(miss)  
3.0
5:With a given list L, write a program to print this list L after removing all duplicate values with original order reserved.
Example: If the input list is 12 24 35 24 88 120 155 88 120 155 Then the output should be 12 24 35 88 120 155 Explanation: Third, seventh and ninth element of the list L has been removed because it was already present. Input Format: In one line take the elements of the list L with each element separated by a space. Output Format: Print the elements of the modified list in one line with each element separated by a space. Example: Input: 12 24 35 24 Output: 12 24 35

a = [12,24,35,24,88,120,155,80,120,155]

dup_items = set()
uniq_items = []
for x in a:
    if x not in dup_items:
        uniq_items.append(x)
        dup_items.add(x)

print(dup_items)
{35, 12, 155, 80, 24, 88, 120}
