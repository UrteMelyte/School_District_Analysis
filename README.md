# School_District_Analysis

## Overview of Analysis
We're conducting an analysis on a district's high school math and reading test scores. One school's (Thomas High School) ninth grade test scores showed signs of being altered, so we needed to remove these scores and recalculate the analysis.


## Results
- **How is the district summary affected?**
The removal of Thomas High School (THS) 9th grade test scores caused the average math score for the district to decrease by 0.1, from 79.0 to 78.9, while the reading score average stayed the same. The affect is more pronounced in the passing percentages: math saw a decrease of 0.2%, reading 0.1%, and overall 0.3%.
- **How is the school summary affected?**
No other schools are affected by the change, just Thomas High School. If we were to calculate the % passing based on the total population, the % passing would be skewed by the lack of 9th grade test scores. Instead, we replace the THS lines with % passing based off the number of 10th - 12th graders, causing the results to change from 93.2/97.3/90.9 (including 9th grade scores) to 66.9/69.6/65.0 (no 9th graders, using total population) to 93.1/97.0/90.6 (just 10th-12th graders).
- **How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?**
Thomas High School's ranking is  not affected by the removal of 9th graders, as they remain #2 within the district.
- **How does replacing the ninth-grade scores affect the following:**
  - **Math and reading scores by grade:** the only change is in THS's 9th grade averages, which are blank due to the lack of 9th grade data.
  - **Scores by school spending:** Once rounded/formatted, there are no apparant changes in the summary by school spending. 
  - **Scores by school size:** Once rounded/formatted, there are no apparant changes in the summary by school spending. 
  - **Scores by school type:** Once rounded/formatted, there are no apparant changes in the summary by school spending. 


## Summary
The four main changes to the data due to replacing THS ninth grade scores with NaNs were:
- THS school % passing math/reading/overall saw a decrease from 93.2/97.3/90.9 to 93.1/97.0/90.6
- The district summary saw slight decreases in the average math score, and all passing %s
- THS no longer has an average 9th grade test score for math or reading
- All other summaries (by spending, size, or school type) saw decreases in the category THS was in, but this was no longer apparant once the passing %s were formatted to no decimal points. I've provided an example of the pre-formatted changes below.

With THS 9th grade test scores:
![Spending Range_PreFormatting](https://user-images.githubusercontent.com/86527135/127752482-d6f28de7-11e8-42b6-b4ee-f442b612fe3d.PNG)

Without THS 9th grade test scores:
![Spending Range_Challenge_PreFormatting](https://user-images.githubusercontent.com/86527135/127752468-a44f0f77-671c-4a46-bc7f-55af09a1798c.PNG)
