# Wav2Lip AI/ML Challenge Modified Colab

This Google Colab notebook is a modified version of the Wav2Lip lip-syncing model, incorporating additional features and enhancements for an AI/ML challenge assigned by Listed (OpeninApp). The original Wav2Lip model and its modifications by Rudrabha and Justin John can be found at https://github.com/Rudrabha/Wav2Lip and https://github.com/justinjohn0306/Wav2Lip, respectively.

## Colab Link
[Play with the modified Colab](https://colab.research.google.com/drive/10qV307-GOb6lZQp7XDwnxK-TmZKWPIu8?usp=sharing)

## Known Issues and Solutions
1. **Mismatched Video and Audio Duration:**
   - *Issue:* The video duration must be greater than or equal to the audio duration.
   - *Solution:* Loop the video to match the audio duration.

2. **Unwanted Frames in Video:**
   - *Issue:* The presence of frames without human faces may cause errors.
   - *Solution:* An additional video cleaning code removes unwanted frames without human faces.

3. **Blurred Lip Movement in GAN Model:**
   - *Issue:* Wav2Lip + GAN model may exhibit blurred lip movement even without a person in the frame.
   - *Solution:* Use the checkbox to choose between models.

## Modifications and Features
1. **Google Colab Setup:** The Colab notebook includes a setup section for easy installation of required modules, cloning the GitHub repository, and handling audio recording.

2. **Video Cleaning:** A new video cleaning code has been added to extract frames from the input video containing a person's face. This eliminates frames with no faces or partially hidden faces, solving issues related to Wav2Lip and Wav2Lip + GAN.

3. **Audio-Video Sync:** The notebook handles cases where the video duration is shorter than the audio. It loops the video until it matches the audio size, ensuring proper synchronization.

4. **Model Selection:** The notebook allows users to choose between Wav2Lip and Wav2Lip + GAN models for lip-syncing.

5. **Adjustable Parameters:** The parameters `pad_top`, `pad_bottom`, `pad_left`, `pad_right`, and `rescaleFactor` can be adjusted to achieve visually satisfying lip-sync results. The notebook provides flexibility in tuning these values.

## Usage Instructions
1. Execute the Colab notebook by clicking the provided link.
2. Follow the instructions in the notebook to upload or provide the path to your video.
3. Adjust the parameters for optimal lip-sync results based on your video characteristics.
4. Run the notebook to generate the lip-synced video.

## Contents in the Drive Link
The [provided Google Drive link](your_google_drive_link_here) contains the following:
- **Input Video:** The original video provided for lip-syncing.
- **Input Audio:** The audio file corresponding to the input video.
- **Intermediate Cleaned Video:** Video frames extracted after cleaning, ensuring only frames with a person's face are included.
- **Output Lipsync Video (Final):** The final lip-synced video generated by the model.


## Feedback and Support
If you encounter any issues or have feedback, please feel free to raise an issue on the [GitHub repository](https://github.com/Tejesh-JP/Tejeshwav2lipmod/) associated with this Colab notebook.

**Note:** This Colab notebook focuses on the AI/ML challenge requirements and modifies only the executable code. Credits for the base Wav2Lip model go to Rudrabha and Justin John.

**Disclaimer:** This notebook is provided as-is, and the user is responsible for adhering to licensing agreements and terms associated with the original Wav2Lip model and its components.
