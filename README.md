# Image-Haze-Removal-using-Dark-Channel-Prior

Introduction
=
This is the Github page for Image Haze Romoval using Dark Channel Prior, which is the project of the course *Digital Image Processing (EE326)* in *Southern University of Science and Technology (SUSTech)*. <br>
The language we use is *MATLAB* with software in version *MATLAB 2017b*.

Project Timeline
=
2018/5/9
-
* Determine the topic of this project

2018/5/14
-
* Finish reading the first and second paper in "Relative Papers" section.

2018/5/18
-
* Finish the first version of the whole program, including:<br>
Dark channel computation<br>
Atmospheric light estimation<br>
Transmission estimation<br>
Guided filtering<br>

2018/5/23
-
* Finish reading the third paper in "Relative Papers" section.
* Improve the performances in "DarkChannel.m" and "AtmosphericLight.m".

2018/5/26
-
* Finish reading the fourth paper in in "Relative Papers" section.
* Improve the performance in "MinFilt.m" and VanHerkMin.m".
* Classify the files of this project into different documents.

2018/5/28
-
* Add "RMSE.m" and "main_score.m" to create a method to evaluate the quality of dehazing algorithm in different parameters or methods
* Add a new method to calculate atmospheric light A based on image entropy.

2018/5/29
-
* Using "RMSE.m" and "main_score.m" to evaluate the performances (time consumption & RMSE score) of different parameter settings.

2018/5/31
-
* Visualize the crude statistics in performance analyses as graph.
* Write scripts and make PowerPoint for presentation.

Relative Papers
=
* *Single Image Haze Removal Using Dark Channel Prior*, Kaiming He, Jian Sun, and Xiaoou Tang, Fellow, IEEE
* *Guided Image Filtering*, Kaiming He, Member, IEEE, Jian Sun, Member, IEEE, and Xiaoou Tang, Fellow, IEEE
* *A fast algorithm for local minimum and maximum filters on rectangular and octagonal kernels*, Marcel van Herk
* *A review on dark channel prior based image dehazing algorithms*, Sungmin Lee1, Seokmin Yun1, Ju-Hun Nam2, Chee Sun Won1 and Seung-Won Jung

Other Supporting Materials
=
* FRIDA (Foggy Road Image DAtabase)
* *An Adventure of Sorts–Behind the Scenes of a MATLAB Upgrade*, Bill McKeeman, MathWorks and Loren Shure, MathWorks
* About the image data type in MATLAB and their conversions: http://www.cnblogs.com/Allen-rg/p/6236009.html (website in Chinese)

Result Demonstration
=
![Result 1](https://github.com/CharlesThaCat/Image-Haze-Removal-using-Dark-Channel-Prior/blob/master/result1.jpg)<br>
![Result 2](https://github.com/CharlesThaCat/Image-Haze-Removal-using-Dark-Channel-Prior/blob/master/result2.jpg)<br>
![Result 3](https://github.com/CharlesThaCat/Image-Haze-Removal-using-Dark-Channel-Prior/blob/master/result3.jpg)<br>

Perfomance Analysis 
=
Time consumption when using van Herk's algorithm in dark channel construction
-
![Time consumption when using van Herk's algorithm in dark channel construction](https://github.com/CharlesThaCat/Image-Haze-Removal-using-Dark-Channel-Prior/blob/master/performance%20analysis%201.png)<br>
Time consumption when using patch based for loop in dark channel construction
-
![Time consumption when using patch based for loop in dark channel construction](https://github.com/CharlesThaCat/Image-Haze-Removal-using-Dark-Channel-Prior/blob/master/performance%20analysis%202.png)<br>
Average RMSE for different dark channel patch size using different methods
-
![Average RMSE for different dark channel patch size using different methods](https://github.com/CharlesThaCat/Image-Haze-Removal-using-Dark-Channel-Prior/blob/master/performance%20analysis%203.png)<br>
Time consumption for different atmospheric light calculation method in patch size 15
-
![Time consumption for different atmospheric light calculation method in patch size 15](https://github.com/CharlesThaCat/Image-Haze-Removal-using-Dark-Channel-Prior/blob/master/performance%20analysis%204.png)<br>
Average RMSE for different atmospheric light patch sizes
-
![Average RMSE for different dark channel patch size using different methods](https://github.com/CharlesThaCat/Image-Haze-Removal-using-Dark-Channel-Prior/blob/master/performance%20analysis%205.png)<br>