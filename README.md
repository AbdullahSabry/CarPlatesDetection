# CarPlatesDetection

The project was fully made by me; Abdullah Sabry. It's attempting to read Egyptian car plates with arabic numbers.

The data used is fully collected by me through the streets of cairo, and carefully labeled each plate in the images to capture:
1) The plate dimension coordinates itself in the image
2) Label the character coordinates within each plate
3) Cut each character and classify it through a classifiaction model

I attempted using two APIs; First of which was the TFObjectDetection API. Using the centernet_resnet50_v2_512x512 for the detection of plates, and characters within
each plate. Classifying these plates used a regular tensorflow classification model for the letters after rescaling.

The second API used was the YOLOv5 which was used in the same order as the TFOBjectDetection for the detection of plates and characters. However used the same
classification model which was used in the TF API; using a conversion library the TF model was converted into a PYtorch model for classification

The results for each API can be found in their consecutive folders in the repo
