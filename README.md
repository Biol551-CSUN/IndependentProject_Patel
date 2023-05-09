# IndependentProject_Patel
This repository contains all the information about my independent project for Computer Modeling class BIOL 551.

### Purpose of choosing this dataset

![](https://opportunitydesk.org/wp-content/uploads/2019/08/7-Guidelines-for-Choosing-the-Most-Suitable-College.png)

College tuition data is somewhat difficult to find - with many sites limiting it to online tools. Being an international student, it was quite difficult for me to choose which university is the best for pursuing my education. There are many websites available online that can guide you, however, if the data from multiple sources is put together, it will enhance your search of universities. This is exactly what I have done for my independent project. 


### Data and Source of data
I chose to work with one of the Tidy Tuesday data sets, **Tuition, diversity and pay.** 

The data comes from many different sources but originally came from the US Department of Education. The most comprehensive and easily accessible data cames from [Tuitiontracker.org](https://www.tuitiontracker.org/). It has a massive amount of data, I have filtered it down to a few tables as seen in the attached .csv files.

There are multiple data available which can be compared to enhance your search. I will be focusing on only these three:

- _historical_tuition_ : *Historical averages* from the [NCES](https://nces.ed.gov/fastfacts/display.asp?id=76) - cover 1985-2016.

- _tuition_cost_ : *Tuition and fees* by college/university for 2018-2019, along with school type, degree length, state, in-state vs out-of-state from the [Chronicle of Higher Education](https://www.chronicle.com/interactives/tuition-and-fees).

- _salary_potential_ : *Salary potential* data comes from [payscale.com](https://www.payscale.com/college-salary-report/best-schools-by-state/bachelors/new-hampshire).


### Data Dictionary

# `historical_tuition.csv`

|variable     |class     |description |
|:------------|:---------|:-----------|
|type         |character | Type of school (All, Public, Private) |
|year         |character | Academic year |
|tuition_type |character | Tuition Type All Constant (dollar inflation adjusted), 4 year degree constant, 2 year constant, Current to year, 4 year current, 2 year current |
|tuition_cost |double    | Tuition cost in USD |


# `tuition_cost.csv`

|variable             |class     |description |
|:--------------------|:---------|:-----------|
|name                 |character | School name |
|state                |character | State name |
|state_code           |character | State Abbreviation |
|type                 |character | Type: Public, private, for-profit|
|degree_length        |character | 4 year or 2 year degree |
|room_and_board       |double    | Room and board in USD |
|in_state_tuition     |double    | Tuition for in-state residents in USD |
|in_state_total       |double    | Total cost for in-state residents in USD (sum of room & board + in state tuition) |
|out_of_state_tuition |double    | Tuition for out-of-state residents in USD|
|out_of_state_total   |double    | Total cost for in-state residents in USD (sum of room & board + out of state tuition) |


# `salary_potential.csv`

|variable                  |class     |description |
|:-------------------------|:---------|:-----------|
|rank                      |double    | Potential salary rank within state |
|name                      |character | Name of school |
|state_name                |character | state name |
|early_career_pay          |double    | Estimated early career pay in USD |
|mid_career_pay            |double    | Estimated mid career pay in USD |
|make_world_better_percent |double    | Percent of alumni who think they are making the world a better place |
|stem_percent              |double    | Percent of student body in STEM |


### Questions to be answered

- **Question #1:** How has the cost of tuition in public and private institutions changed over the years?
OUTPUT 1: Variation in cost of tuition of Private and Public institutions (Year Vs Tuition cost (in USD))

- **Question #2:** How do the institutions in different states differ in their fees, for example, room and board, in-state tuition fees, out-of-state tuition fees, or even total fees? 
OUTPUT 2: State-wise comparison of in-state and out-of-state fees (State Vs Type of fees (in USD))

- **Question #3:** What percentage of students are enrolled in STEM courses in the institutions of a particular state, for example, California?
OUTPUT 3: Percentage of students enrolled in STEM fields in Californian institutions (Percentage Vs Name of the institutions)

### Layout of the project

- Load the libraries
- Load and read in the data
- Filter to remove unwanted variables
- Create a ggplot
- Save it in Output folder

### Additional references
- Github link for the data: https://github.com/rfordatascience/tidytuesday/tree/master/data/2020/2020-03-10
- Diversity by college/university for 2014, along with school type, degree length, state, in-state vs out-of-state from the Chronicle of Higher Education.
- Example diversity graphics from Priceonomics.
- Average net cost by income bracket from TuitionTracker.org.
- Example price trend and graduation rates from TuitionTracker.org


### Thank you!
