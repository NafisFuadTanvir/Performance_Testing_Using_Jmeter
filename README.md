## Performance Test Requirements:- 
Load Test server Link:-  https://restful-booker.herokuapp.com

## Test_Scenario: 120,000 users over a 12-hour period. log in, create a booking, and search for the booking.

Todo 1 : Find the throughput and perform a load test (you can limit the load test to a maximum of 20 minutes to save time) to ensure the server can handle the load. Create a load test report.
Use a Gaussian Random Timer (Deviation 2000ms, Constant delay 500ms). Do it in 3 step 1st step: 5 min load 2nd step: 10 min load 3rd step: 20 min load.

Todo 2 : If the load test passes, identify the bottleneck throughput by conducting a stress test. Create a stress test report. 

Todo 3 : Generate an HTML report for both the load test and the stress test. Also add the steps for both load test and stress test into 2 excel tab named load test report and stress test report. 

## JMETER THREAD :- 
<img width="497" height="499" alt="image" src="https://github.com/user-attachments/assets/55b42802-7dbf-4367-853a-cc9cf73d9b58" />

## How to Run The project?
First save the Jmx file, and open it in Jmeter. Then add the neccessary Headers, Gaussian Timer, Random Variables and User Defined Variables.

Here is the login url:- https://restful-booker.herokuapp.com/auth . Body: { "username": "admin", "password": "password123" }

Here is the Create Booking url:- https://restful-booker.herokuapp.com/booking .Body: { "firstname": "Generate Random FirstName", "lastname": "Generate Random LastName", "totalprice": Generate random amount, "depositpaid": true, "bookingdates": { "checkin": "2024-01-01", "checkout": "2024-01-02" } }

Here is the search url:- https://restful-booker.herokuapp.com/booking/<booking_id>.

## Result 

Request summary of Load Test:-

<img width="1885" height="757" alt="image" src="https://github.com/user-attachments/assets/6b3879e8-c49f-4ffa-b07e-f83dee8a895e" />

statistics of Load Test:- 

<img width="1680" height="796" alt="image" src="https://github.com/user-attachments/assets/b0176d07-e625-4582-9adb-1dd7326cb5ad" />

Excel Preview of Load Test:-

<img width="1152" height="749" alt="image" src="https://github.com/user-attachments/assets/cb9a0bf9-044b-47a0-a5e8-63fa164c1e34" />


