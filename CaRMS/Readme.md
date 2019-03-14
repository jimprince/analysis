# CaRMS Project

## Overview

Every year medical graduates are matched to Medical Residency positions across Canada through the Canadian Residency Matching Service (CaRMS). In recent years the number of students who are left without a position at the end of the match has risen. Of most concern is that those that are left without a position are qualified physicians who have passed all their courses and exams and have been deemed competent to enter residency, leading to the concern that it is not a problem with the quality of the students but of the match system itself to efficiently allocate student-residency pairs.

There have been numerous explainations for the increase in unmatched students, from a decline in number of residency positions, medical students demonstrating a stronger preference for limited or competitive disciplines, or simply denial stating that recent changes in the number of unmatched students is a statistical aberration. 

This project will evenutally be compiled into an aricle for publication, and seeks to answer a few key questions:

1. Is the match rate different than 10 years ago in a statistically significant manner. Is every school statistically different?

3. Which variables appear to be most sensitive (sensitivity analysis) to changing the national unmatched student rate.

4. Are there situations which lead to a non-linear decrease in the efficiency of the match?

2. Does the number of residency positions offered by a school affect the match rate of that school's students (probably will use the top 5 schools according to UGME:PGME ratios and bottom 5 schools comparing them using a T test). 

At the core of this analysis will be a numerical simulation designed to approximate the complex relationship between the variables and outputs. This will be trained on all data until the last 10 years. Validation will take place over the last 5-10 years of data in order to tune the parameters of the model and then a final test set of the last 5 years will be used to test the ability of the model to generalize to data it hasn't seen. After that, the idea is that common solutions to the unmatched medical student can be trialed using this simulation to estimate their effects on the unmatched student.

Numerical methods to approximate the real life phenomenon of the match are by their nature limited in their precision and, like a chisel, leave characteristic marking on their product. Though the tool is imperfect, the hope is that some insight can be generated to help increase the efficiency of the Canadian residency match.



## Questions:

1. Why do we care about unmatched medical students/ match efficiency?
    1. A year lost in physician training
    2. Obligation to students to provide post-graduate training
    3. Public accountability for public subsidy of medical education
    4. cost of match to students
    5. Stress of match on students and their health
    6. **It is a far more efficient system to have qualified healthcare professionals working as service providers for a year rather ran repeat an already academically successful year or take time away for graduate training.**
1. Where do unmatched students come from?
2. What strategies are used for the match
    1. Undifferentiated applicant who is average and apply to a specialty (estimate 25-30%). 
        1. Competitive
        2. Non-Comptetiive
        3. Maybe a backup
    2. Apply to Location
    2. Apply to a discrete specialty
    3. How many other specialties you apply to
    4. How many other locations you apply to
2. Types of applications
    1. Reasonable iters, no flags
    2. Rare fields (fields that don't have an obvious backup)
        1. Radiology
        2. Public Health
        3. Genetics
        4. Optho
        5. Pathology
2. Does a global increase in the number of applications actually reduce the unmatched rate? (prisoner's dilemna)
2. Which specialities are competitive
3. Does the number of PGME positions affect match rate from that school
4. Can numerical methods be used to build a reasonable model of the canadian match
5. Using that model
    1. What is the optimum ratio of students to positions
    2. What is the optimal number of positions to add, and at what schools
    2. How does the length of ROL affect the liklihood of matching
    3. Is it possible to predit the next year's match based on this year's match results
    4. What are the effects of an internship year
    5. What are the effects of training everyone as a family doc
    6. What are the costs associated with unmatched medical students
    7. What are the costs of interviews tour based on how effective the match is.
6. What is the motivation of each of the parties
    1. UGME
    2. PGME
        1. Fill program with excellent people and good fit
        2. Whether or not they have to go unmatched in first or second iteration
        
    3. CaRMS
    4. Students
    5. Public
    
## Observations

1. For a student togo unmatched they either have to:
    1. Not be ranked by the schools that they interview at
    2. The programs fill up before they find the student on their ROL
    3. IF there are fewer empty positions at the end of the match than in previous years, that would suggest the first as a cause of an increase in unmatched students.
2. Umatched rate has gone up despite a significant increase in ROL and number of applications per student
3. There has not been rigorous analysis yet published in a peer reviewed journal on the subject of the unmatched medical student, though much of the data is easily accessible.
4. Economical concerns will primarily care about the number of unmatched students after the second iteration of CaRMS, whereas emotional effects, stress, and cost of applications are more likely to focus on unmatched students after the first iteration of CaRMS
5. Many students do not seem willing to enter a family practice residency 
6. 2011 -> quebec brought into the match (3-4:1 from quebec: to quebec)
7. 2011-2016 -> Governments increased med school spots and kept residency positions constant or decreased them 
8. (15-16 -> double digits unmatched)
9. Go fish strategy, displace people with weakers applications, but not nessesarily weaker CVs
10. Increase in volume has decreased quality of review, significantly increased quantity of work. 
11. Decrease in quality of student applications because they are working on so many
12. Program cycle
    1. Radiology in 2011 super high unmatched to 2017 with unmatched spots because of horror stories about unmatched in previous years

## Possible Solutions to the match
1. Increase number of residency positions
2. Internship year for students unsure of what specialty they would like to pursue or are pursueing a competitive specialty
3. Limit number of applications
4. We're going to fail a certain number of medical students. Not everyone who gets into the program graduates
5. Every program has to rank every student in the country and every student has to rank every program in the country which would result in zero unmatched
6. Add ties and optimize for lowest -> score programs instead of rank programs (either allocating a fixed number of points or assigning each school a score)
    1. (1) program A
       (1) program B
       (1) program C
       (5) program D
       (8) program E
    2. (1)
    3. Decreased cost to faculty
    4. Decreased cost to Students
    5. Theoretical increase in match rate
7. Flexible number of PGME positions based on the number of applicants or number of applicants that are 

## Other Complaints
1. In a publicly funded system medical students should be required to be wiling to work as a family physician as the public has a significant investment in their educaiton and so the public has a right to have that student as a service provider (corner case for people who will leave medicine if they don't get their specialty of choice).
    1. Primarily directed at students interested in competitive specialties. Competitive specialties also tend to be the highest paid specialties. The majority of the cost of these specialties is in physician wages (citation needed). Basic economics of supply and demand dictates that increasing supply ofyour most expensive component, while keeping demand constant, naturally leads to a marketplace where the price drops. The result is that more people are serviced for the same cost with an increase in the number of physicians in a dicipline (should be. It may be the case that increasing the supply of physicians may activate latent demand, or unmet demand, in the which case supply increases, demand increases, the cost per unit remains the same, but overall cost increases. On second thought, using a simple economic model to predict population demand for a given service may not be comprehensive enough a view. Supply and demand also requires that customers have variable price sensitvity as a prerequisite for use. As the person who pays is not the same person who is consuming the service and determining demand, the basic laws of supply and demand don't apply, which seems sad that such a useful model doesn't provide any meaningful insights in this case.)
2. Cost to the school is really big

## Future Work
1. Include location preference when students are ranking programs
2. Add match strategies to students
    1. How does the proportion of students with a given strategy affect the overall match
3. Physician pay by country as it relates to the number of medical students graduated