# trachoma_grading_kappa_ODK

This ODK form is designed to present a series of curated images of trachoma to field graders. 
In the choices sheet of `trachoma_grading_kappa.xlsx` you will see the choice list `reference`.

This stores the expert data which provides the reference information for the photo, plus any additional notes that you want to show up on screen.

The prototype here has 10 questions. 

To increase the number of questions

* Copy the Q0001 block.
* Paste below the last question and above the `results` group
* Select the new block of rows. 
* Use find and replace to replace the text `Q0001` with whatever the new one is, i.e. `Q0011`
* In the `image` column, change the name of the image to i.e. `Picture11.png`
* To make all the calculations work, add the new questions to the fields `count_tp`, `count_tn`, `count_fp`, `count_fn` and `count_correct`
* Save the form and upload to ODK Central
* Test it, check kappa scores make sense

## Features

* Only the first selected answer is recorded. Changing the answer is not recorded after the first press.

* Calculates observed and expected agreement, as well as Kappa Scores

* Saves all values to ODK Central

## Roadmap

* ruODK/Quarto scripts to 
	* monitor and create dashboard
	* evalate whether specific photos are systematically misclassified
* Confidence intervals on Kappa etc.





