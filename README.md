# Arabic Image Captioning and Question Answering App 

## Table of Contents  
- [Overview](#overview)  
- [Features](#features)
- [Tech Stack](#Tech-Stack)
- [Workflow](#workflow)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Technologies Used](#technologies-used)  
- [License](#license)  

## Overview  

This repository contains the code for an AI-powered application that generates captions for images, translates them into Arabic, and answers user-submitted questions in Arabic.  


### Key Components:  
1. **Image Captioning**: Generates descriptive captions for input images.  
2. **Arabic Translation**: Translates captions from English to Arabic.  
3. **Audio Playback**: Converts Arabic captions to speech for playback.  
4. **Visual Question Answering (VQA)**: Answers questions about the image in Arabic.  

---

## Features  

- **Image Captioning**  
   - Generate captions for uploaded images using advanced AI models. 

- **Caption Translation**  
   - Translate captions into Arabic for regional users. 

- **Audio Generation**  
   - Converts Arabic captions into speech for audio playback or download.  

- **Question Answering**  
   - Answer user-submitted questions about the uploaded image.

- **Interactive Interface**  
   - Built with Gradio for a seamless user experience.

---

## Tech Stack  
- **Python**  
- **Hugging Face Transformers**  
- **BLIP Models**  
- **gTTS**  
- **Gradio** 

---

## Workflow  

Here’s breakdown of the application system:  

1. **Input Image**: User uploads an image via the Gradio interface.  
2. **Caption Generation**: The image is processed to generate an English caption using a BLIP-based model.  
3. **Arabic Translation**: The caption is translated to Arabic using a pre-trained translation model.  
4. **Audio Output**: Arabic captions are converted to speech using Google Text-to-Speech (gTTS).  
5. **Question Suggestions**: The model generates suggested questions related to the image. Users can select or input custom questions.  
6. **Visual Question Answering (VQA)**: The selected question is answered, and the answer is translated into Arabic.  
7. **Result Display**: Both the Arabic caption and the VQA answer are displayed.  

---

## Installation  

To set up this project locally, follow these steps:  

1. **Clone the repository**  
    ```bash  
    git clone https://github.com/ayahani59/Arabic_Image_Captioning_App.git
   cd Arabic_Image_Captioning_App
    ```  

2. **Install required libraries**  
    ```bash  
    pip install -r Requirements.txt  
    ```  

3. **Run the app**  
    ```bash  
    python app.py  
    ```  

4. **Access the interface**  
   Open your browser at `http://127.0.0.1:7860` to interact with the app.  

---

## Usage  

1. Upload an image via the Gradio interface.  
2. The pipeline generates an English caption, translates it to Arabic, and provides an audio playback option.  
3. Select a suggested question or input a custom question about the image.  
4. Receive the answer in Arabic, both as text and audio.  

---

## Technologies Used  

- **[BLIP Image Captioning Models](https://huggingface.co/Salesforce/blip-image-captioning-large)**: For generating image captions.  
- **[MBART Translation Models](https://huggingface.co/facebook/mbart-large-50-many-to-many-mmt)**: For Arabic translation.  
- **gTTS**: For converting Arabic text to speech.  
- **Gradio**: For building an interactive user interface.  

---

## License  

This project is licensed under the MIT License. See the [LICENSE](LICENSE.txt) file for details.  
