By: Arda Cifci, Tushrima Kelshikar, Zihan Yu


Note: 
Hello Professor or TA(s), Our group was given a deadline extension to Wednesday April 17th at 11:59 pm by Dr. Lim through e-mail
due to a emergency situation from a group member.



The structure of your code and dataset so that the TA can easily navigate your project:

Opening our Project folder you will see five folders and a README file. The Dataset folder contains our dataset 
raw video samples and the annotations that came from our processing. Inside the “Classification_csv” folder you 
will see three CSV files containing our dataset’s annotations. The “Video_Samples” folder contains the videos 
sorted by their culture/country. Back at the home folder, The “Misc” folder contains files used for our plots 
and can be ignored.  The “Preprocessing” folder contains the processing files needed to extract the annotations / data 
needed to classify a new video.  You will need to run a new video through all three processing files before we can classify. 
The “Test_Video” file contains a sample processed video used to test the classification. The “Classify” folder contains
our classifier file. After running the processing files you would then place the resulting csv files into this classification 
file for the final results. Our analysis and other results are in this file aswell. You shouldn’t need to install 
any special dependencies (besides jupyter notebooks and the imports) to run this file.


A self-evaluation of your project with respect to your proposal:

In our project proposal we stated that being able to recognize the different social signals for different sub-categories of fear
would be meaningful and was one of our main aspects of our project. Additionally, we also wanted to focus on recognizing the 
cultural social signal difference that came alongside these fear sub-categories.  Originally we wanted to do more than three 
sub-categories of fear but due to only using 200 video samples any more sub-categories would result in worse and worse 
accuracies in our classifiers. In our proposal we also stated we would explore using SVM’s or KMeans to classify our results 
but these proved to be too low in accuracy. We pivoted towards using neural networks and multi-layer perceptrons to classify 
our data as these resulted in higher accuracies. Overall, we accomplished what we said in our proposal but we wish our accuracies 
classifying the different cultures and subcategories were higher. If we were to do this program again we would collect a lot more 
than 200 video samples.  



Special dependencies:

There are three special dependencies required for our project, 

1. The first one would be Jyupter notebooks. All our code is programmed using Jyupter notebooks. You can install Jyupter 
notebooks following the instructions here:  https://jupyter.org/install

2. OpenPose is required to process videos into body keypoint features.  To install OpenPose please follow the directions 
here: https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md  
Depending on which operating system your computer is you would need to follow different installation instructions. 
IMPORTANT NOTE: Currently OpenPose’s download server web addresses for specific parts of the installation are not functional.  
Therefore, unless you are using a windows machine and can run the pre-built windows CPU version, you might not be able to install OpenPose at this time.

3. OpenFace is required to extract facial features from videos. To install OpeFace, follow the instructions 
here: https://github.com/TadasBaltrusaitis/OpenFace 
I used a MAC, the feature extraction command cmd = f'./FeatureExtraction -f "{video_path}" -out_dir "{output_folder}"'

4.FFmpeg is required to transfer our videos to mp3 files. To install FFmpeg, follow the instructions here: https://ffmpeg.org/download.html. 
I used MacBooks, the command cmd = ffmpeg -i ‘video name.mp4’ ‘video name.mp3






