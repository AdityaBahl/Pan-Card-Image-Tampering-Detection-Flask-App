# PAN Card Image Tampering Flask App

## Colab File

For reference or for a better understanding in a step by step manner(but purely Python Code)
https://colab.research.google.com/drive/1OGq8HlQuYADtiVQ7f5Pg4dz6FAiy6ubA?usp=sharing

## Technologies Used

1. **HTML**
2. **CSS**
3. **JavaScript**
4. **Python**
5. **Flask**

## Getting Started

**_Step to run application:_**

1. **Create the copy** of the project.
2. Open **command prompt** and change your current path to folder where you can find **'app.py'** file.
3. **Create environment** by command given below-

   ```
   conda create -name <environment name>
   ```

4. **Activate environment** by command as follows-
   ```
   conda activate <environment name>
   ```
5. Use command below to **install required dependencies**-
   ```
   python -m pip install -r requirements.txt
   ```
6. **Run application** by command;
   ```
   python app.py
   ```
   You will get **url** copy it and **paste** in browser.
7. You have **'sample_data'** folder where you can get **images to test**.

## Why PAN card Image Tampering Detection Flask App?

A **_PAN card Image Tampering Detection Flask App_** can be used to detect if a PAN card image has been tampered with. PAN (**Permanent Account Number**) cards are government-issued identification cards that are used for tax-related purposes in India. Tampering with a PAN card image could be used to commit fraud or other illegal activities, so it's important to be able to detect any tampering that may have occurred. A Flask App can be used to create a user-friendly interface for users to upload and check their PAN card images, making the process of detecting tampering more convenient and accessible.

## Modules

1. **_Flask_**(1.1.1)
2. **_imutils_**(0.5.3)
3. **_Keras_**(2.4.0)
4. **_opencv-python_**(4.4.0.46)
5. **_Pillow_**(8.0.1)
6. **_tensorflow_**(2.3.1)
7. **_scikit-image_**(0.17.2)

## Algorithm

1. **Open Image** and **display** the file format of the source file.
2. **Resize** the Image
3. **Change image format** to png(If required).
4. **Load** the two input images(original and tampered) into imread function of cv2(open cv).
5. Convert the images to **grayscale**
6. Compute the **_Structural Similarity Index (SSIM)_** between the two images, ensuring that the difference image is returned. Structural similarity index helps us to determine exactly where in terms of x,y coordinates location, the image differences are. The **_lower_** the SSIM score, the **_lower_** the similarity.
7. Loop over the **contours**.
8. **Visualise images** using different functions and display original image with contour
9. Display tampered image with **contour** and **black and white** images respectively.

## Challenges and Limitations

There are several challenges and limitations that may arise when developing a PAN card Image Tampering Detection Flask App:

1. **_Image quality:_** The app must be able to handle images of varying quality, such as those taken with a smartphone camera or those that have been scanned.

2. **_Tampering detection:_** The app must be able to accurately detect tampered images, which can be difficult if the tampering is subtle or not easily visible to the naked eye.

3. **_False positives:_** The app may generate false positives, where it incorrectly identifies an image as tampered even though it is not.

4. **_False negatives:_** The app may generate false negatives, where it fails to identify that an image has been tampered.

5. **_Security:_** The app must be secure, as it will be handling sensitive personal information such as PAN numbers.

6. **_Scalability:_** The app must be able to handle a large number of image uploads and processing at the same time.

7. **_Maintenance:_** The app must be regularly updated to ensure that it is able to detect new forms of tampering and to fix any bugs or issues that may arise.

8. **_Privacy:_** The app must comply with all relevant privacy laws and regulations.

9. **_Limited Data:_** The model will be trained on limited data and therefore the accuracy is limited.

10. **_Limited model performance:_** The model has a limited performance and will not be able to detect all the tampering.

11. **_Limited resources:_** The app may be limited by the resources available, such as computing power and storage.

Overall, it's important to keep in mind that developing a Pancard Image Tampering Detection Flask App is a complex task that requires a variety of skills and knowledge in image processing, machine learning, and web development.

## Conclusion

In conclusion, a **_PAN card Image Tampering Detection Flask App_** can be a useful tool for detecting tampered PAN card images and preventing fraud and other illegal activities. However, there are several challenges and limitations that must be considered when developing such an app, including image quality, tamper detection accuracy, false positives and negatives, security, scalability, maintenance, and compliance with privacy laws and regulations. Additionally, the app may be limited by the resources available, such as computing power and storage, and the model may have limited performance and accuracy due to limited data. Despite the challenges and limitations, a Pancard Image Tampering Detection Flask App can help to improve the security and integrity of PAN card images and the government's identification process.

### MIT Licence

**Copyright (c) 2023 Aditya Bahl**

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
