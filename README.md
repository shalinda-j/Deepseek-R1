# Deepseek-R1
Using Google Colab to Run the DeepSeek R1 Model on Your Own Server

If you want to use the DeepSeek R1 model on your own server via Google Colab, follow these steps:

Step 1:
Open Google Drive and create a new folder.

Step 2:
Open the newly created folder, right-click inside it, go to the More tab, and create a Google Colab project.

Step 3:
Now, paste and run the following commands in your Colab notebook:

python
Copy
Edit
!pip install langchain  
!pip install langchain-core  
!pip install langchain-community  

!pip install colab-xterm  
%load_ext colabxterm  
%xterm  

curl -fsSL https://ollama.com/install.sh | sh  

ollama serve & ollama run deepseek-r1:7b  
Once the installation is complete, you will be able to use the DeepSeek R1 model on your own server.
