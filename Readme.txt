## Indian Semi Acted Facial Expression Database (iSAFE)

ISAFE is one of it's kind database for human emotions. 

Human emotion recognition is of par importance for human computer interaction. Dataset and it's quality plays important role in this domain. In this paper we propose a new dataset which contains **395 clips of 44 volunteers** between 17 to 22 year of age. All the clips are manually splitted from the video recorded during stimulent clips are watched by volunteers. Facial expressions are self annotated by the volunteers as well as cross annotated by annotators. Analysis of the dataset is done using Resnet34 neural network and baseline for the dataset is provided for research and comparison. 

Emotion mapping:

#1 Happy 
#2 Sad 
#3 Surprise 
#4 Disgust 
#5 Fear 
#6 Angry 
#7 Uncertain 
#8 Noemotion
 
Folder structure in database:

Database : Dataset of images
	| S0XX : Folders corresponding to each subject (volunteers).
		| XX : Folders containing frames of sequence for an emotion of subject after removing blurry frames.
		| XX.mp4 : video files for an emotion of subject.

Handcrafted Features: Dataset of features extracted from images
	| S0XX : Folders corresponding to each subject (volunteers)
		| XX : Folders containing histogram of oriented gradients (hog), csv and avi file of boxed position of feature point on face

Annotations: Contains annotions which maps session of subjects with respective emotions
	annotation.csv : CSV file for annotations done by non profesional annotator.
	psy-annotation.csv : CSV file for annotations done by profesional annotator (phsycolgist).
	self-annotation.csv : CSV file for annotations done by volunteers (subject) themself.
	
Structure of CSV:

subjectNumber/expressionSequence , emotionValue
To know more about the database read [this](https://link.springer.com/chapter/10.1007/978-981-15-4828-4_13) paper.
