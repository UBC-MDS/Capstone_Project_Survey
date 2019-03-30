# Proposal

For this project we were asked to conduct a survey of our MDS class and teaching fellows in order to apply our knowledge of causal inference and experimentation in a simulated real-world setting.

Given we recently had to rank projects for the capstone course, which is an important and exciting part of this program for likely all of the students, we decided to explore the factors that led students to decide on their top-ranked project. Specifically, our group chose to investigate whether a student's perceived skill level with statistics or machine learning influenced their decision to rank a statistics or machine learning problem as their top-ranked project. We are interested to see whether students chose to rank project they are more comfortable with completing well, or whether they viewed capstone as an opportunity to improve their skill in the area they are weaker in. Obviously there are many factors that may have led students to decide on a particular capstone project, and as such we will add questions to our survey to look for confounding variables.

*__Research question__: Does an MDS student's perceived skill level with statistics or machine learning influence their decision to rank a (mainly) statistics or machine learning project as their top choice for capstone?*

### Main survey questions

Since we are interested in collecting information about two perceived skills as our predictors (X variables), we will ask the following survey questions:
1. On a scale of 1-10 what is your perceived skill-level with solving statistical problems?
2. On a scale of 1-10 what is your perceived skill-level with solving machine learning problems?

To obtain data about the response variable we will ask students which capstone project was their top choice. On the backend we will classify the projects as being either a statistics or a machine learning project. By framing the question in this way, we hope to minimize any inferred bias that may come from directly asking respondents about whether their top choice project was statistics vs. machine learning. Thus our final survey question to obtain data about the response is:
1. Which of the following capstone projects was your top choice:
- *drop down list of all project - only one can be selected**

### Confounding variables

We plan to ask the following questions to look for confounding factors (answer options and reason for question outlined):
1. What is your age?
- choices: drop down menu of binned age categories
- reason: there may be age group differences in the interest with a project types (e.g. younger student may prefer statistics)
2. What is your gender?
- choices: man, woman, other
- reason: gender difference may explain project choices
- reason: there may be gender differences in project interests (e.g. woman prefer machine learning)
3. How many years of post-secondary education did you complete?
- choices: list with integer values
- reason: different years of education may be associated with different interests (e.g. more years of school associated with enjoying statistics)
4. Please rate your interest level with statistics subject matter on a scale of 1-10?
- choices: list of integer values
- reason: student with interest in statistics may have chosen a statistics project
5. Please rate your interest level with machine learning subject matter on a scale of 1-10?
- choices: list of integer values
- reason: student with interest in machine learning may have chosen a statistics project
6. How many formal post-secondary courses in statistics did you complete?
- choices: free text integer
- reason: attempt to quantify actual skill level which may be a confounding factor to choosing a particular project type
7. How many formal post-secondary courses in computer science did you complete?
- choices: free text integer
- reason: attempt to quantify actual skill level which may be a confounding factor to choosing a particular project type
8. Do you have any work experience with machine learning?
- choices: Yes, No
- reason: attempt to quantify comfort level with machine learning problems; students may have chosen a project based on comfort with subject
9. Do you have any work experience with statistics?
- choices: Yes, No
- reason: attempt to quantify comfort level with statistics problems; students may have chosen a project based on comfort with subject
10. What is your perceived difficulty of your top choice capstone project?
- choices: Low, medium, high
- reasons: students may have chosen a project based on difficulty
11. Did you perceived your top choice capstone project to be in a supportive company?
- choices: Yes, No
- reason: students may have chosen a project based on how much support would be available to successfully complete the task
12. Did you choose your top choice capstone project because there was a possibility to be employed by them afterwards?
- choices: Yes, No
- reason: students may have chosen a project because they viewed it as an employment opportunity

### Analysis plan:

We will use a logistic regression to determine how perceived skill level with statistics influenced students to choose a statistics capstone project. We will use a second logistic regression model determine how perceived skill level with machine learning influenced students to choose a machine learning capstone project. We will check to coefficients of the regression models for significance. We do not perceive that we will need to adjust any p-values as we are looking at only two relationship in the dataset. We chose to use a logistic regression model as our response variable is binary and thus we expect it to be well modelled by a binomial distribution.

To examine for confounders, we will first check whether there was any variation in the questions testing for confounders. If there is significant variation, we will have to control for it using stratification as this is an observational study.

### Reflection on UBC Office of Research Ethics document on Using Online Surveys  

Our survey will not collect directly identifying information such as name, student number and SIN number. What we will collect are MDS students' choices of capstone projects, their ages, their education backgrounds, etc. Even though a single variable on its own could not identify an individual, variables combined may expose individuals to identification. In consideration of this risk, we will treat all information collected as "personal information" and manage it according to the guidelines outlined below.  

As such, according to the BC Freedom of Information and Protection of Privacy Act (FIPPA), we should store the information we collect only in Canada and only access in Canada. To comply with it, we decided to use a Canada based online survey tool to conduct our survey.  

According to FIPPA, an IP address constitutes indirectly identifying information. Since we have no interest in survey respondents' IP addresses, we will switch off the IP tracking feature provided by the survey tool.  

If it important to enable a participant to make an informed decision about participating in our online survey. To achieve this goal, we need to include a cover letter in our survey. In this cover letter, we will include: the study title, contact information of the PI, a short description of the study, risks and benefits, limits to confidentiality, a statement that participation is optional, and the UBC Research Participant Complaint Line text.
