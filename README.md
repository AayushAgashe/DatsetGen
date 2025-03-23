**AI-Generated Synthetic Dataset Creator**
This project is a Google Colab notebook that generates synthetic text using a pre-trained GPT-2 model from Hugging Face. It can be used for creating artificial datasets for machine learning model training.

**Features**  
✅ Uses Hugging Face's transformers library  
✅ Generates synthetic text based on a prompt  
✅ No API key required  
✅ Runs on Google Colab for free  

**How to Use**  
1.Open the notebook in Google Colab  
2.Run all cells to set up the model  
3.Enter a custom prompt to generate synthetic text  
4.Save the output for dataset creation  

**Installation**  
Run the following command in a Colab cell if needed:     
!pip install transformers  

**Example Usage**  
from transformers import pipeline

text_generator = pipeline("text-generation", model="gpt2")

prompt = "AI is transforming the world by"
generated_text = text_generator(prompt, max_length=50, do_sample=True)[0]['generated_text']

print(generated_text)  

**Contributing**  
Feel free to open issues or suggest improvements!

**License**  
This project is for educational purposes.

