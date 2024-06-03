- # llama 3 Vs Chat GPT 3.5

</br>
<img src="./llama3_Vs_GPT_3_5.png">
</br>

- # 1. Introduction :
  - ### 1.1 Objective :
    - This project aims to compare the responses from Two diffrent large language models : llama3 and Chat GPT 3.5 turbo
  - ### 1.2 Specs :
    - llama3 : installed on local machine the latest 8b model @ 06/03/2024
    - Chat gpt : using a private API key, the model is gpt-3.5-turbo
  - ### 1.3 Installation :
    - llama3 :
      - Link to Ollama tool : <a href="https://ollama.com/download">Ollama</a>
      - Link to the llm model : <a href="https://ollama.com/library/llama3">llama3</a>
      - After installing the ollama tool : download model by the following command
        - ollama run llama3
    - Gpt :
      - How to use gpt : you need to have a subscription to use their API
      - Call the OPENAI api : you need to add a payment method to avoid api limit reached error code 429
        - Click here <a href="https://platform.openai.com/playground" >API Dashboard</a>
        - After the payment is added, go to usage section on left panel and see if the bar is green, which means you can call the api
- # 2. Test Scenarios :
  - The <a href="https://github.com/SouLayman2022/llama3_Vs_Gpt_3.5">repos</a> contains a page saved as a pdf, link to real website <a href="https://www.caranddriver.com/tesla/model-3">link</A>
  - We wwill be using both models to see which one of them gets the response right, in regards of the prompts at the end of this notebook, promyts used are below :
    - questions = [
      "What topic the document is about ?",</br>
      "What is the name of the website in the document ?",</br>
      "What is name of the car ?",</br>
      "What is the price of the car ?",</br>
      "What is the year of production of the car ?",</br>
      "How much HP does the car have ?",</br>
      "How much time it takes the car to reach 60 mph ?",</br>
      "How much is the range of the car ?",</br>
      "How much is the the fuel rating of the car ?",</br>
      ]
  - The MODEL variable holds the llm models names, so comment llama3 if you want to use gpt, else leave it as is the run llama3 instead
- # 3. Running the notebook :
  - open the file PDF_RAG.ipynb on your IDE, Vscode... or use the command on cmd like this :
    - git clone https://github.com/SouLayman2022/llama3_Vs_Gpt_3.5.git
    - cd llama3_Vs_Gpt_3.5
    - python -m venv llama3_requirements
    - llama3_requirements\Scripts\ativate
    - pip install -r requirements.txt
    - jupyter notebook
    - a web page contaning the noteboo will be shwon double click the : PDF_RAG.ipynb to open it
    - after finishing running or twiking do following commands :
      - pip freeze > requirements.txt ( save your installed packages )
      - deactivate ( to opt out of venv )
