# R-shiny-app



**Tab1=Home** :
The home page of the Diabetes Readmission calculator provides a tabular representation of the data for exploratory analysis. It helps to select just a subset of the data given certain conditions on characteristics of patients.

**Tab2= Drug and Demographics** :
The dosage for 24 key medicines are represented through a bar chart. We chose this over a normal column graph so that the names of all drugs are clearly visible. To enable this simplified representation of this data, data was transposed using reshape library in R. This helped us to represent the data in a cumulative bar chart as shown. Each stack in the bar chart represent variation in dosage after the admission â Up,Down or Steady. This can give some clear inferences, like that the most commonly used medicine is insulin and that though for majority of patients the dosage remains steady, there is notable change as well â both Up and Down.Relation between time spent in hospital and age is represented through a scatter plot. It can be seen above that younger population generally stays in hospital for a lesser time compared to the older patients.A whisker plot is used to display the summary statistics related to Race and time spent by them in hospital. It can be inferred from above that Asians tend to spend higher time,while Hispanics spend the lowest time in hospital compared to others.

**Tab3=Readmission Calculator** :
The user selects values for inputs such as time the patient spent in the hospital, age, race, gender of the patient, along with the primary diagnosis. On click of âPredictâ button,readmission calculator displays the probability of readmission of the patient. This is when the inputs are used to score the probabilities using the Decision tree model already built. The process happens in real time and takes a little while to process and display the output to the user. The probabilities which indicate danger are indicated in red, while the probability of no readmission is indicated in green.
