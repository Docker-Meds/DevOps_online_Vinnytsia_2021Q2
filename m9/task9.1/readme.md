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
	if number%5==0 and number%3==0:  
		return 'FizzBuzz'  
	elif number%3==0:  
		return 'Fizz'  
	elif number%5==0:  
		return 'Buzz'  
	else:  
		return number    

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
	
3. ### Calculator
class calculator:  
 def add(self, a, b):  
   return a+b  
 def subtract(self, a, b):  
   return a-b  
 def multiply(self, a, b):  
   return a*b  
 def divide(self, a, b):  
   return a/b  
	
4. ### Calculator test
import unittest  
from calculator import calculator  
class TestCalculator(unittest.TestCase):  
  def setUp(self):  
    self.calculator = calculator()  
  def test_add(self):  
    self.assertEqual(self.calculator.add(4,7), 11)  
  def test_subtract(self):  
    self.assertEqual(self.calculator.subtract(10,5), 5)  
  def test_multiply(self):  
    self.assertEqual(self.calculator.multiply(3,7), 21)  
  def test_divide(self):  
    self.assertEqual(self.calculator.divide(10,2), 5)  
if __name__ == "__main__":  
  unittest.main()  
  
  
![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m9/task9.1/images/2.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m9/task9.1/images/3.PNG)

![images](https://github.com/Docker-Meds/DevOps_online_Vinnytsia_2021Q2/blob/Master/m9/task9.1/images/4.PNG)

