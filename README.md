# Pclub_task3
Drive link :https://drive.google.com/drive/folders/1cNSw_eawYD-KAeNkLj7GVsGxxIL5mnke?usp=drive_link
This drive link contains the zip file of my dataset

Approach : Now my dataset was UTK dataset of which I have attached the link .In this datset the females are labelled 1 and male 0. This dataset was of people's faces without any covers, so the major challenge was to train the model for masked faces. To tackle this problem  I reasearched a bit about face detection models and came to know about haarcascade. Now firstly I created another dataset folder "Face_detected_dataset" in which I detected the faces and then cropped them out and saved in this folder. Then I crosschecked again using haarcascade and deleted the files in which there were no faces in the folder "Face_detected_dataset". Now I deduced that a face usually covers 40 percent of our face so I again created another dataset folder "Cropped_face_dataset" where I croped the bottom 40 percent of every image in our folder "Face_detected_dataset" . 
Now finally I used "Cropped_face_dataset" as my dataset and trained my model according to this. Now I extracted the labels 1 or 0 from the "Cropped_face_dataset" and then added it to an np array and then I trained the model with these labels which are essentially the genders and the images. After this for testing I again used haarcascade and detected face then cropped the bottom 40 percent and then tried to predict the gender. After this I took approx 100 masked images and labelled them and then I tried to predict their gender and compared it to their labels and calculated the accuracy which is 65 percent .I have added these test faces to my google drive. 

Screenshots:
![All the deleted pictures which were not detected using haarcascade](https://github.com/Ikrima248/Pclub_task3/assets/153128448/5b2cb85a-fad9-46e8-b0a3-fe1b0e16d39d)
![bottom 40 cropped ](https://github.com/Ikrima248/Pclub_task3/assets/153128448/b8a076bc-dff4-4e88-a8c2-23eae2acb4a9)
![Model training 2](https://github.com/Ikrima248/Pclub_task3/assets/153128448/53b956![Model Training ](https://github.com/Ikrima248/Pclub_task3/assets/153128448/1ef7d334-2618-46f5-a9a3-4ad84f074dee)
1d-9d0c-4617-9baa-2f2e67201fcc)
![Test and accuracy screenshot ](https://github.com/Ikrima248/Pclub_task3/assets/153128448/9390abf3-e2ba-4702-aa6b-66e26d749e12)
