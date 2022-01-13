# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

![image](https://user-images.githubusercontent.com/88845919/149055826-d2558906-cfdf-45ae-afa2-c108a9ccbc6e.png)
This is the summary of the linear regression to predict MPG

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
The Vehicle_length and the Ground_clearance are statistically unlikely to provide random amounts of variance to the linear model.

- Is the slope of the linear model considered to be zero? Why or why not?
![image](https://user-images.githubusercontent.com/88845919/149056417-fc8231c3-5a32-4919-ab85-e16f23239315.png)
No, we can notice that the slope of the linear model is not zero, this means that a correlation exist between this variables and the MPG.

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Yes, R-squared is 0.7149, so we can say that ther exist a strong correlation between the variables and the MPG

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

Total Summary

![image](https://user-images.githubusercontent.com/88845919/149060682-7797b8e4-fce4-4873-b526-eb11a4e9d447.png)

Lot Summary

![image](https://user-images.githubusercontent.com/88845919/149060719-6fca3baf-630b-447f-98b4-b13b8783ee9e.png)

We can see that the in group, statistically, the coils match with the requirement. The variance is 62.3. But when we separate with lot, we can notice that this value is affected when we take a bigger sample. Actually the Lot3 doesn´t math the requirement, the variace is 170.29.

## T-Tests on SuspensionCoils

RScript using the t.test() function to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.

![image](https://user-images.githubusercontent.com/88845919/149067537-82b28f54-1e1e-4099-8d95-3cda184b9351.png)

On the general analysis with T test, we can see that the mean is different from 1,500. Probably there is a lot that has a difference. We can spect from previous analisys that Lot3 could have this difference.

![image](https://user-images.githubusercontent.com/88845919/149067569-d5bb2bb6-f569-4457-973c-897c67fbc1f3.png)

Is the see the analysis for lot 1, we can see that it matches with 1500, so it's ok.

![image](https://user-images.githubusercontent.com/88845919/149067606-33529153-db7e-4dcd-8cd9-749a66aebd17.png)

The Lot 2 has a small difference.

![image](https://user-images.githubusercontent.com/88845919/149067649-6b8a9292-0419-405f-8f30-9c780fa6925a.png)

But lot 3 has the bigger difference in the mean, so this lot doesn´t match the requirement, probably this will be scrap and manufacture again.

## Study Design: MechaCar vs Competition

- What metric or metrics are you going to test?

Thinking on a comparison with the competition, I think that some importants metrics to track are: cost, security raiting, comfort raiting, fuel efficiency, type of car.

- What is the null hypothesis or alternative hypothesis?

H0: It's not posibble to offer a car with a low cost, less than $ 10,000 dls and have high comfort, security and fuel efficiency.
Ha: It's possible that a car with a cost less than $ 10,000 dls can offer high comfort, security and fuel efficiency.

- What statistical test would you use to test the hypothesis? And why?

Multiple Linear Regression, to relate different variables to the cost of the car and idenfity if there's and area of oportunity. With this we ca prioritize the high cost characteristic and get a good idea of what to consider for the design.

- What data is needed to run the statistical test?

We need diffent models, types of cars, with their cost, security ratings, create a comfort raiting and fuel efficiency.
