# SubjectiveTermsRewriter
A Pipeline for detecting and improving the Subjective Sentences in SRS docs improving the clarity and quantifiability. 

Solution:
A precompiled vague-lexicon was used to detect vague terms in sentences. The flagged sentence was prompted to gemini-ai for rewriting the sentence into precise, quantifiable sentence.

Instructions for running the code:
1️. Prerequisites
You need:
A Google account (for Colab and Drive access)
Access to Google Colab
A valid Google Gemini API key(can be obtained via google cloud ai)

Get it from: https://aistudio.google.com/app/apikey

2. Folder Setup (in Google Drive)

Create the following structure in your Drive:
MyDrive/
      └── NLP_ASG/
           ├── Data/
           │    ├── raw_txt/       ← Original PURE dataset files
           │    └── Cleaned/       ← Preprocessed .txt files
           ├── Outputs/
           │    ├── Vague_Rewrites.csv
           │    ├── Vague_Term_Frequency.csv
           │ 
           └── Subjective_Term_Detector.ipynb
           
3. Running the code(jupiter notebook)
Open "Subjective_Term_Detector.ipynb" file from ur drive, which directs to google collab platform.
Then Mount your drive and make sure to have the above mentioned folder structure.
Then change the file paths whenevr requiredaccording to your drive structure.
After doing above  steps start running the code cells sequentially.

On end go to the outputs folders and analyse the csv files for vague sentence and its rewritten form. 

