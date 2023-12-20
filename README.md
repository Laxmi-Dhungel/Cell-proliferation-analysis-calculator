This project works like a calculator to analyze the cell proliferation data.
Cell proliferation experiments are conducted to test effectiveness of different drugs or in varying concentrations of single drugs against cells (e.g. cancer cells).
The experiment design for this type of assay includes 96 well plates. Some of the wells on the plate are treated with drugs and some are left untreated (control). 
After certain time (depends on study), the optical density (OD) on each well is measured that corresponds to the cell viability. Higher OD corresponds to higher viability and lower OD corresponds to lower viability (higher killing by drug).

Traditionally, these data are analyzed by averaging OD for the controls (average control OD) then OD on all wells are divided by the average control OD and then multiplied by 100 to obtain percentage survival.
percentage survival= (OD for the treatment/average OD for control)*100

The percentage survival for each treatment groups are averaged to get mean percentage survival. These information on mean percentage survival can be either plotted on excel ir using some other software. Some further work needed include calculation of standard deviation and computing p value for each treatment compared to control. The information on standard deviation and statistical significance need to be plotted on figure. Uff.. too much of work.

However, the code generated here requires only few minutes to generate a bar graph displaying percentage survival along with standard deviation and statistical significance. Further it also provided options to users to transfer the csv file on percentage survival in case needed for future. The user need to input few information that include file name, control name, image title and labels.

Now, I am going to explain the data format and how to run the code for the analysis.
Attached is the sample plate design for the cell proliferation experiment. C represents control (untreated cells) and numbers represent different concentrations of drugs.


<img width="459" alt="96 well plate" src="https://github.com/Laxmi-Dhungel/Cell-proliferation-analysis-calculator/assets/154451345/50a43d34-ee35-439d-ac55-45e1bea33047">


The OD values obtained for each treatment is shown in figure. The csv file to be loaded should be in this format where first row represent different treatment groups.  
<img width="398" alt="OD values_cell proliferation" src="https://github.com/Laxmi-Dhungel/Cell-proliferation-analysis-calculator/assets/154451345/b2c4cbf6-baff-4b6f-b634-94b1603a480e">

When the code is run, user will be asked to input the file name at first. Here, I have input file name as cell_proliferation_assay.csv.

<img width="432" alt="input_file_name" src="https://github.com/Laxmi-Dhungel/Cell-proliferation-analysis-calculator/assets/154451345/b17e46cc-7541-4a99-8173-64b3f0c83429">

Then the user will be asked to input control name. And on next step, users will be asked to input title, x and y labels for the image.

<img width="421" alt="title_labels" src="https://github.com/Laxmi-Dhungel/Cell-proliferation-analysis-calculator/assets/154451345/95c69ebb-53d2-47e4-805e-339120b392b6">

After user provide this input, barplot on the percentage survival with information on statistical analysis is generated. 
![cell_proliferation_bar_graph](https://github.com/Laxmi-Dhungel/Cell-proliferation-analysis-calculator/assets/154451345/75a834cf-6cf3-4fba-b974-5b3a181ebcdb)

Then user will be asked if they want to transfer the csv file that include data on percentage survival. If typed 'yes' then user are asked to type the name of csv file they want to create. After pressing enter, a csv file containing data on percentage survival is created.  

<img width="468" alt="csv_file_write" src="https://github.com/Laxmi-Dhungel/Cell-proliferation-analysis-calculator/assets/154451345/d910e040-36d0-4496-bd49-ba0ffd477866">

And at the end, user are aksed if they want to analyze next set of data. 

<img width="395" alt="continue_analysis" src="https://github.com/Laxmi-Dhungel/Cell-proliferation-analysis-calculator/assets/154451345/b494fd76-b68c-4e63-9fdb-9fc051986edf">


Isn't this as easy as using a calculator? :)


