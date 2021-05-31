### Myocardial Echocardiography Dataset (MCE) for effort prediction

This overall dataset was created from real clinial exams acquired at Guangdong Provincial People’s Hospital. Acquired data were fully anonymized. Our dataset contains MCE sequences of A4C chamber from 130 patients, each sequence contains 30 frames isometrically sampled from the raw DICOM file, all images are center cropped to a fixed dimension 512x512. The dataset consists of both CAD and healthy subjects, whose diagnosis results are extracted from clinical medical cases (though the diagnositic label is not given). MCE sequences of all subjects are collected by an ultrasonography system (Philips 7C and iE ELITE，Philips Medical Systems, Best, Netherlands) equipped with a broadband transducer, and SonoVue (Bracco Research SA, Geneva, Switzerland) as the contrast agent.

The dataset can be divided into two parts. The first part is from subject_000 to subject_099, only one MCE sequence exist for each subject. The frames of these 100 subjects are annotated by an experienced cardiologist using [Labelme](https://github.com/wkentaro/labelme) tool. This part is used for training our segmentation network and effort prediction network in our paper. The second part is from subject_100 to subject_129, more than one MCE sequence exist for each subject. The frames in this part do not have segmentation annotation, they are used for testing the performance of our effort prediction network. 

If you used our dataset, please consider to cite our paper "Towards Efficient Human-Machine Collaboration: Real-Time Correction Effort Prediction for Ultrasound Data Acquisition".

Some examples are shown below.

![](example.png "example images in the dataset")
