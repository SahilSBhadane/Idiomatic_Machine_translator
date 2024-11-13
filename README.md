# Idiomatic_Machine_translator

- This project focuses on training a custom translation model using a dataset of English and Hindi idioms, built and fine-tuned using Google Colab.

## 🚀 **Project Overview**
This project aims to build a custom machine translation model from scratch using NLP techniques. The project includes:
- Training a custom tokenizer using SentencePiece.
- Fine-tuning a transformer-based model using the `MarianMTModel` architecture.
- Translating idiomatic expressions from English to Hindi (in Romanized script).

## 📂 **Repository Structure**
```
.
├── English_Hindi_Idioms_Romanized.csv  # Dataset used for training
├── fine_tuned_mt5                      # Trained model checkpoints
│   ├── config.json
│   ├── generation_config.json
│   ├── tokenizer_config.json
│   ├── special_tokens_map.json
│   ├── model.safetensors
│   ├── spiece.model
├── notebook.ipynb                      # Google Colab notebook
└── README.md                           # Project documentation
```

## 🛠️ **Setup Instructions**

### **Step 1: Clone the Repository**
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### **Step 2: Install Dependencies**
Make sure you have the necessary packages installed. You can install them using:
```bash
pip install -r requirements.txt
```
> **Note**: If you're running this on Google Colab, most dependencies like `transformers`, `torch`, and `sentencepiece` should already be available.

### **Step 3: Open the Colab Notebook**
1. Upload the `notebook.ipynb` to Google Colab.
2. Run the cells sequentially to train the model, save the tokenizer, and generate translations.

## 📊 **Dataset**
The dataset used in this project is `English_Hindi_Idioms_Romanized.csv`, which contains idiomatic expressions in English and their corresponding translations in Hindi (Romanized).

**Dataset Example**:
| English Idiom        | Hindi Equivalent (Romanized)        |
|----------------------|------------------------------------|
| Cut corners          | shortcut apnana                    |
| Break the ice        | barf todna                         |
| Burn the midnight oil| raat bhar jagna                    |
| Piece of cake        | bahut aasan kaam                   |

## ⚙️ **Model Training**
- The model is trained from scratch using `transformers` and `sentencepiece`.
- The architecture is based on the MarianMT model, modified to fit the custom tokenizer and dataset.
- The model is fine-tuned for 10 epochs with a learning rate of `5e-5`.

## 🖥️ **Usage**
After training, you can test the model using the `translate_idiom()` function.

```python
# Example translation
print(translate_idiom("Cut corners"))  # Expected output: "shortcut apnana"
print(translate_idiom("Break the ice")) # Expected output: "barf todna"
```

## 🛠️ **Technologies Used**
- Google Colab
- Hugging Face Transformers
- SentencePiece
- PyTorch

## 🤖 **Model Performance**
> Include a summary of your model's performance, accuracy, or any observations here.

## 🔮 **Future Enhancements**
- Expand the dataset to include more idioms and phrases.
- Experiment with different model architectures for improved translation accuracy.
- Integrate a web interface for real-time translation.

## 🤝 **Contributing**
Feel free to submit pull requests to enhance this project. If you have any questions or suggestions, open an issue!

## 📝 **License**
This project is licensed under the MIT License.

## 📞 **Contact**
- **Your Name** - sahilbhadane04@gmail.com
- **GitHub**: https://github.com/SahilSBhadane
