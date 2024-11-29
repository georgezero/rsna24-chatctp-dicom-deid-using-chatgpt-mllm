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
- [Presentation](https://drive.google.com/file/d/1fpCwhNB6JHphbP1z2kSBOXLCOQB2SEuO/view?usp=drive_link)

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

**DICOM Tags Exploration with ChatGPT**
- DICOM Metadata Tags with (Fake) PHI using GPT
   - [Example 1](https://chatgpt.com/share/6747d0fd-393c-800e-bb32-07e8688f19e9)
   - [Example 2](https://chatgpt.com/share/6747d108-70e4-800e-a95e-105e6e82b111)
- Radiology Report Deidentification with (Fake) PHI using GPT
   - [Example 1](https://chatgpt.com/share/6748643d-5ed0-800e-a714-acb1395d56d9)
   - [Example 2](https://chatgpt.com/share/67486455-7098-800e-b5c3-679258b9f383)


:bulb: Example prompts:
- *DICOM Metadata*
   - Tell me about a bit about the patient and the exam performed.
   - Analyze the DICOM metadata and give me all the values that contains personal health information. Show this in a table format.
   - Identify all the DICOM metadata containing potential personal health information (PHI). These can be directly identifying information (such as name, unique ID, etc) or indirectly identifying information (such as demographic, other ID, etc). Do not include fields that does not have a PHI risk such as technical details. Show this in table format with the field name and value.
   - Deidentify the DICOM metadata containing personal health information using fake information. Show the values before and after in table format.
   - Anonymize all the potential personal health information in the DICOM metadata. Show the values before and after in table format.
- *Radiology Report*
   - Analyze the radiology report and give me a list of all the personal health information
   - Anonymize all the potential personal health information on the radiology report

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

This URL forwards to the latest Google Colab notebook for DICOM DeID coded by ChatGPT - [Colab notebook](https://colab.research.google.com/drive/1-q99nLG2-oC3P5BjDrPS7JXVpOS0VrEq?usp=sharing)

:bulb: Example of python notebook output:

![example-chatgpt-output](images/6.%20Appendix/example-chatgpt-output.png)


