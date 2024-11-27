# RSNA 2024 - DeID using ChatGPT and Multimodal LLMs (MLLM)

## Deep Learning Lab Session - DLL08

### Tuesday, Dec 3
### 11:00 AM - 12:00 PM CST
### DEEP LEARNING LAB

## Speakers

- George Shih
- Adam Flanders
- Errol Colak
- Hui-Min Lin
- Chinmay Singhal


## Outline

### 1. Session Intro - George

### 2. DICOM intro (DICOM tag deid issues) - Errol

### 3. *NEW* DeID tools from RSNA - Adam
- [Presentation](https://drive.google.com/file/d/1ESB_y9whSxuIUgTPO-IGyvT4aTjAGiIA/view?usp=sharing)
- RSNA Anonymizer2
   - Available for download on the RSNA Github page:
      - https://github.com/RSNA/Anonymizer
   - Other RSNA research tools
      - https://www.rsna.org/research/imaging-research-tools
- Report De-identifier
   - HuggingFace
      - https://huggingface.co/StanfordAIMI/stanford-deidentifier-with-radiology-reports-and-i2b2
   - GitHub Repository
      - https://github.com/MIDRC/Stanford_Penn_MIDRC_Deidentifier
   - MIDRC Tools
      - https://www.midrc.org/algorithms
   
### 4a. [Hands-On] DICOM Tags Exploration with LLMs - Hui-Ming

**DICOM Tags Exploration with ChatGPT and other LLMs**

(pre-DeID) [CHATGPT LINK]

(post-DeID) [CHATGPT LINK]

:bulb: Example of DICOM tags exploration with LLMs:

![image]()

### 4b. [Hands-On] DICOM Image with (Fake) Burned-in PHI Exploration with Multimodal LLMs - Chinmay

**Using ChatGPT Vision Model (GPT-4o) to examine radiology images with burned-in PHI**

- [Hands-on Link](https://rsna.md.ai/reporting/share/report_XrgqexKGxm)


:bulb: [Example images](images/4b.%20[Hands-On]%20DICOM%20Image%20exploration/) with fake burned-in PHI:

| Chest Xray  |  Ultrasound   |  CT Abdomen  |
|:-----------:|:-------------:|:------------:|
|[![chest-xray](images/4b.%20[Hands-On]%20DICOM%20Image%20exploration/chest-xray.png)](images/4b.%20[Hands-On]%20DICOM%20Image%20exploration/chest-xray.png) | [![ultrasound](images/4b.%20[Hands-On]%20DICOM%20Image%20exploration/ultrasound.png)](images/4b.%20[Hands-On]%20DICOM%20Image%20exploration/ultrasound.png) | [![ct-abdomen](images/4b.%20[Hands-On]%20DICOM%20Image%20exploration/ct-abdomen.png)](images/4b.%20[Hands-On]%20DICOM%20Image%20exploration/ct-abdomen.png) |

### 5. [OPEN SOURCE LLMs] Using local Multimodal LLMs for PHI detection on images - George

:bulb: Llama3.2-Vision-11b

<img width="1702" alt="image" src="https://github.com/user-attachments/assets/7d05a88c-6672-4716-ae86-9f7906f21b4c">

<br/>
<br/>

[Using Open Source Local Multimodal LLMs (SLIDES)](https://docs.google.com/presentation/d/e/2PACX-1vTXn8hMDJihlYWl1oUB2fhnCQIM0BXzRXsNh6sx7K0wE3UYEQYVkAS8DH1ZxYAvYis_qQKa5nVeloS1/pub)

**REFERENCES:**

#### Ollama (LLM server)

https://ollama.com/

#### Open WebUI (Web app used with Ollama)

https://openwebui.com/

#### Anything LLM (Desktop app used with Ollama)

https://anythingllm.com/

#### LM Studio (Desktop App / LLaMA.cpp as LLM server)

https://lmstudio.ai/

#### Collama (Ollama + Google Colab -- free GPU)

https://github.com/5aharsh/collama/

#### Tutorial: Install Ollama + Open WebUI on Mac / Linux / Windows (WSL)

https://www.saltyoldgeek.com/posts/ollama-llama3-openwebui/

### 6. Wrap-Up - George / Adam

---

### Appendix

#### Use ChatGPT to generate a python script to deid DICOM tags

This URL forwards to the latest Google Colab notebook for DICOM DeID coded by GPT-4.

https:/

:bulb: Example of python notebook output:

![image]()

![image]()



