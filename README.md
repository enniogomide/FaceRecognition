# **FaceRecognition**

## Description

This work was carried out in three stages.

## **Steps**

### Step 1:
use of the face_recognition.py library, the purpose of which is to store the parameters (encoding data) based on a photo of the person so that it can be used as a basis for identifying the person.

This is on the notebook: **FaceRecognition_HOG**

Details of the implementation and how to run it are in the notebook itself.

### Step 2:
Validating the result using the webcam.

The process is carried out for a single person. The identification of several people in the photo has not been implemented, but it is possible.

notebook: **FaceRecognition_HOG_webcam**

### step 3:

Trying to seek greater generalization, since the above process requires cross-referencing each enconding with all those registered for identification. We haven't done a volume test, but we'll probably have an impact.

To try to minimize this, we set up a network using structured data, but the result was very low, showing that we would need more images, to review the network settings or even the model used.

notebook: **FaceRecognition_Structured_data_classification**

## **Considerations**

in the folder we have:
photos used in webcam validation.

**faces_encoding_parameters** - the data that identifies the people who were part of the assembly process.

BarackObama, DonaldTrump, KeanuReeves

**faces_names** contains the names of the people whose data we are encoding.

**encoding_faces_with_class** contains the encoded data and the classes (target) of each person for training the structured network.

### Folder for validation

For validation, you need to create the **ImagesValidation** folder, with subfolders containing the same names (written in the same way) as in the training process.
