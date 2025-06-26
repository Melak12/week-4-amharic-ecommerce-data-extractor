# Week 4 -  Building an Amharic E-commerce Data Extractor
Transform messy Telegram posts into a smart FinTech engine that reveals which vendors are the best candidates for a loan.

### Business Need
EthioMart has a vision to become the primary hub for all Telegram-based e-commerce activities in Ethiopia. With the increasing popularity of Telegram for business transactions, various independent e-commerce channels have emerged, each facilitating its own operations. However, this decentralization presents challenges for both vendors and customers who need to manage multiple channels for product discovery, order placement, and communication.

To solve this problem, EthioMart plans to create a single centralized platform that consolidates real-time data from multiple e-commerce Telegram channels into one unified channel. By doing this, they aim to provide a seamless experience for customers to explore and interact with multiple vendors in one place.

This project focuses on fine-tuning  LLM’s for Amharic Named Entity Recognition (NER) system that extracts key business entities such as product names, prices, and Locations, from text, images, and documents shared across these Telegram channels. The extracted data will be used to populate EthioMart's centralised database, making it a comprehensive e-commerce hub.

### Key Objectives: 

- Develop a repeatable workflow that begins with data ingestion from Telegram channels, proceeds through preprocessing and labeling, and results in structured, machine-readable data.
- Fine-tune a transformer-based model to achieve high accuracy (measured by F1-score) in identifying Product, Price, and Location entities within unstructured Amharic text.
- Go beyond just building a model by comparing multiple approaches, interpreting your model’s predictions with tools like SHAP/LIME, and delivering a final analysis that recommends the best model for EthioMart's business case.

### Possible entities 

- Product Names or Types
- Material or Ingredients: Specific mentions of materials used in the products.
- Location Mentions
- Monetary Values or Prices

**Optional entities to be collected**
DELIVERY_FEE: To capture transaction costs beyond the product price.
Examples: "free delivery", "150 birr delivery fee", "delivery cost extra".
CONTACT_INFO: To capture the means of completing a transaction.
Examples: Phone numbers (09...), Telegram usernames (@username).


## Setup
1. Clone: `git clone https://github.com/Melak12/week-4-amharic-ecommerce-data-extractor`
2. Create venv: `python3 -m venv .venv`
3. Activate: `source .venv/bin/activate` (macOS/Linux) or `.venv\Scripts\activate` (Windows)
4. Install: `pip install -r requirements.txt`

Note: if requirements.txt is missing, you might need to run this command
`pip freeze > requirements.txt`
