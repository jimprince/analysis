# CaRMS Project

## Overview

Every year medical graduates are matched to Medical Residency positions across Canada through the Canadian Residency Matching Service (CaRMS). In recent years the number of students who are left without a position at the end of the match has risen. Of most concern is that those that are left without a position are qualified physicians who have passed all their courses and exams and have been deemed competent to enter residency. 

There have been numerous explainations for this pattern from a decline in number of residency positions, medical students demonstrating a stronger preference for limited or compettive disciplines, or a simply denial stating that recent changes in the number of unmatched students is simply a statistical aberration. 

This project will evenutally be compiled into an aricle for publication, and seeks to answer a few key questions:

1. Is the match rate different than 10 years ago in a statistically significant manner

3. Which variables appear to be most sensitive (sensitivity analysis) to changing the national unmatched student rate

2. Does the number of residency positions offered by a school affect the match rate of that school's students (probably will use the top 5 schools according to UGME:PGME ratios and bottom 5 schools comparing them using a T test). 

At the core of this analysis will be a numerical simulation designed to approximate the complex relationship between the variables and outputs. This will be trained on all data until the last 5 years. Validation will take place over the last 5-10 years of data in order to tune the parameters of the model and then a final test set of the last 5 years will be used as final validation of the model. After that the idea is that common solutions to the unmatched medical student can be trialed to estimate their effects on the unmatched student.

Numerical methods to approximate the real life phenomenon of the match are by their nature limited in their precision and, like a chisel, leave characteristic marking on their product. Though the tool is imperfect, the hope is that some insight can be generated to help increase the efficiency of the Canadian Resident Matching Service.



Questions:

1. Where do unmatched students come from?
2. What strategies are used for the match
    1. Apply to a specialty
        1. Competitive
        2. Non-Comptetiive
    2. Apply to Location
    3. How many other specialties you apply to
    4. How many other locations you apply to
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
    3. CaRMS
    4. Students
    5. Public