n# CensusPrediction
In hospitals, patients are admitted and discharged on a daily basis. Currently there is a fixed number of physicians who admit and
discharge these patients on daily basis. Those physicians are called **hospitalists**.
If there is a surge in the patients who need to be admitted, that will create a strain on the hospitalists who may become understaffed to take care of the extra number of patients. On average, a hospitalist can see 16 to 20 patients a day, so if there are 5 hospitalists a day in a given hospital and one day the number of patients in the hospital is 120, that number of patients or **census** creates an extra burden of 4 patients for each hospitalist. That could lead to inadequate and suboptimal care.
Being able to predict the next day's census, allows hospitalists team to be adequately staffed by calling in an extra physician the day before.
In this project, I analyse the dataset of daily census and how it varies over the year, and in the end I use the *ordinary least square* from scipy to predict the next day's census based on today's census data.
*Census.csv* represents the main dataset, *Backup.csv* shows the days when a "backup" physician was called in, "day8" represents an extra physician already scheduled ahead of time to work on that day. I was curious to know whether having a backup and/or an extraphysician (day8) would increase the number of discharges.
*Total.csv* is the combination of "census.csv" and "backup.csv".
*Newcc.csv* and *Ccols.csv* are the result of manipulating and shifting the columns of *census.csv* in order to have today on the same row as tomorrow for predictive purposes. "Today" represents today's census, "Tomorrow" represents tomorrow's census and "PriorDis" represents today's discharges.
