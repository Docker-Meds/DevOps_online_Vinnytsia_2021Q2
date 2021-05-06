1. ### Fizzbuzz number
def fizzbuzz(number):  
    if number % 3 == 0 and number % 5 == 0:  
         return 'FizzBuzz'  
    elif number % 3 == 0:  
        return 'Fizz'  
    elif number % 5 == 0:  
        return 'Buzz'  
    else:  
        return number  

for number in range(1, 51):  
    print (fizzbuzz(number))  
    
2. ### Fizzbuzz  
def get_reply(number):  
	if number % 5==0 and number % 3==0:  
		return 'FizzBuzz'   
	elif number %3==0:  
		return 'Fizz'  
	elif number %5==0:  
		return 'Buzz'  
	else:  
		return number  
	for number in range(1, 51):  
		print (fizzbuzz(number))  

3. ### Fizzbuzz test
import unittest  
import fizz_buzz  

class FizzBuzzTests(unittest.TestCase):  

def test_fizz(self):  
	number=6  
		
result = fizz_buzz.get_reply(number)  
		
self.assertEqual(result, 'Fizz')  
		
def test_buzz(self):  
	number=10  
		
result = fizz_buzz.get_reply(number)  
		
self.assertEqual(result, 'Buzz')  

def test_fizzbuzz(self):    
	number=15  

result = fizz_buzz.get_reply(number)  
		
self.assertEqual(result, 'FizzBuzz')  
		
if __name__ == '__main__':  
	unittest.main()
	
![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m9/task9.1/images/1.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m9/task9.1/images/2.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m9/task9.1/images/3.PNG)

