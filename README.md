# RUN-ICON
RUN-ICON algorithm for unsupervised learning

## Flowchart of algorithm:

1. A CSV datafile is input

2. Data is read, saved in a numpy array and normalized, based on the max-min values of each column

3. Within RUN-ICON, for every loop, the Generalized Centre Coordinate is calculated for comparisons

4. Frequency of occurrence of most dominant centres is calculated

5. Centres (both normalized and de-normalized) are output in a file for future use

6. The code outputs from 10 different runs the frequency of appearence of dominant clustering configuration (in %) for the "i_cluster" variable, which denotes the number of clusters you want to separate your data in. An average of these 10 values is calculated. This represents the confidence. The higher the mean frequency of occurrence, the higher the confidence.
7. Calculate the difference between the maximum and minimum of the confidence values. This represents the uncertainty. The lower the difference, the lower the uncertainty is.


PLEASE NOTE: If you want to test frequency of occurrence of dominant centres for different number of clusters 
              you must modify variable "i_cluster" manually in the code
 


If you use this software in any publication, please cite the following paper:
Christakis, N.; Drikakis, D. "Reducing Uncertainty and Increasing Confidence in Unsupervised Learning." Mathematics 2023, 11, 3063. https://doi.org/10.3390/math11143063
