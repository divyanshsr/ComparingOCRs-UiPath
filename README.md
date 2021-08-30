# ComparingOCRs-UiPath

This project interprets text images via the system file explorer and utilizes 3 OCR engines to convert images within a folder into respective text files. This enables the user to process images in a compact, efficient and convenient manner. 
This allows the user to easily convert properly scanned images while maintaining the integrity of the document format. This robot helps us in the following ways:
1. It removes the intermediate steps of locating an Image-to-Text conversion website or software.
2. It utilizes three OCR Engines to provide options to the User.
3. It provides a direct interface to the text files, with a distinction as to which OCR engine was used.

Process Definition: 
Images are read from file and the robot uses 3 OCR engines to convert the images into text files. 

Inputs:
Image files present in a folder.

Output:
Text files that are ready to be utilized by the user.

Process Design:
1. The file path is recorded to “imgs” and the number of arguments are recorded to “args”.
2. A loop within the “imgs” begins and the images are being converted to a UiPath.Core.Image object.
3. This object is then converted into the respective text object using three OCR engines, Google Tesseract OCR Engine, Abbyy Cloud OCR Engine and the Microsoft OCR Engine. 
4. Finally, the text objects are flushed to the disk and the task is completed.


