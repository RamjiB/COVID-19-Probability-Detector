## <div align="center">COVID-19 INFECTION PROBABILITY DETECTOR</div>
### Problem:
The cases of COVID-19 are increasing day by day at an exponential rate. In India, although the situation is worth controllable till now, but the number may suddenly outburst someday. In such situation, we might be short of devices or machines for detecting coronavirus.
### Idea:
In such situation, it is necessary to prioritise the patients and patients with more chances of having infection should be tested first.

For example, imagine a situation where 20,000 patients have come for check-up but only 8,000 devices are available. In such scenario, top 8,000 patients with more chance of infection should be given priority because they have more chance of spreading the infection. Others can be tested lately since they might not be infected by the virus.
### Solution:
We can first collect data regarding the age and symptoms of people affected by COVID-19. The actual type of data can be decided by the specialists from medical field. I hereby present just a **sample data which is randomly generated by me for an example**.
S.No. |	Age (in years) |	Body temp. (in °F) |	Fatigue |	Cough |	Body pain |	Sore throat |	Breathing difficulty |	Infected
:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:
|1. |	38 |	99.42 |	1 |	0 |	1 |	0 |	0 |	0 |
|2. |	72 |	104.65 |	1 |	1 |	1 |	2 |	2 |	1 |
|3. |	56 |	102.32 |	0 |	1 |	1 |	0 |	1 |	1 |
|4. |	52 |	102.50 |	1 |	0 |	0 |	1 |	1 |	0 |
|5. |	45 |	98.65 |	0 |	1 |	1 |	1 |	0	| 0 |
|6. |	84 |	101.59 |	1 |	1 |	1 |	0 |	2 |	1 |
|7. |	62 |	103.07 |	1 |	0 |	1 |	0 |	2 |	1 |
|8. |	44 |	100.96 |	0 |	1 |	0 |	1 |	1 |	1 |
|9. |	68 |	100.35 |	1 |	1 |	0 |	2 |	0 |	1 |
|10. |	65 |	102.69 |	1 |	1 |	1 |	1 |	1 |	1 |

**_Note:_** </br>
*	_In the above data, in fields of ‘Fatigue’, ‘Cough’, ‘Body pain’ and ‘Infected’:_ </br>
_0 – No_ </br>
_1 – Yes_ </br>
*	_In fields of ‘Sore throat’ and ‘Breathing difficulty’:_ </br>
_0 – Not at all_ </br>
_1 – Little bit_ </br>
_2 – Too much_ </br>


The above data is just a **randomly generated sample**. Government can avail data for 50,000-60,000 people across globe.

Now a machine learning model can be trained and tested on the data collected, where the ‘features’ will be ‘age’ and ‘symptoms’ and ‘label’ will be ‘probability of patient getting infected’.

So now when a new patient will come, we can simply ask the patient about age and various symptoms and the model will tell the probability of patient being affected. 

For example, if patient gives the information:
1.	Age - 42 years
2.	Body temp. - 102.65 °F
3.	Fatigue - 1
4.	Cough - 0
5.	Body pain - 1
6.	Sore throat - 1
7.	Breathing difficulty - 0

The machine will give output – 46% (**just an example, not by model**)

So, this way the probability of all the patients can be recorded and then sorted in decreasing order simultaneously so that patients with more chance of infection get priority and be tested first.


Whatever discussed till now was about the method of working of model in scientific terms. In common man’s terms, it will be like a software with user friendly interface where patient can fill a digital form asking various details about symptoms. On clicking the submit button, the patient will be able to know the probability of him getting infected by COVID-19.

Although doctors can use this by prioritising the patients, even the people at homes can check their probability of having infection by COVID-19 and can better stay at home instead of going outside and visiting doctor if probability is less than 40% or so. This will also prevent crowd.

### Requirements
To run this system, you should have following requirements in your PC:
1. sklearn
2. numpy
3. django



