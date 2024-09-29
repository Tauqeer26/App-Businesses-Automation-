
# Retail Business Automation System

## Objective
The **Retail Business Automation System** is designed to intelligently process email requests for a retail store. The goal is to automate responses to customer inquiries and order requests, ensuring efficiency in handling customer interactions. The system uses a product catalog and current stock status to provide relevant responses.

## Features
1. **Email Classification**: Classify incoming emails as either a _"product inquiry"_ or an _"order request"_.
2. **Order Processing**:
   - Verify product availability based on stock levels.
   - Fulfill the order if all requested items are in stock.
   - Generate responses to customers indicating whether their order is being processed or if items are unavailable.
3. **Automated Response Generation**: Craft appropriate replies based on the type of email, whether it's an inquiry or an order.

## Project Overview
This project utilizes machine learning and natural language processing techniques to classify emails and interact with product data. The process includes:

- **Product Data Management**: A catalog of products, including fields like product ID, name, category, stock amount, detailed description, and applicable seasons.
- **Email Handling**: An automated pipeline to process a sequence of emails, extracting relevant details such as email ID, subject, and content.

### Main Steps
1. **Classify Emails**:
   - Categorize each incoming email as either a product inquiry or an order request.
   - Update the email classification sheet with columns: `email ID`, `category`.

2. **Process Order Requests**:
   - Check product availability and stock levels.
   - Create an order entry if the order can be fulfilled. If not, notify the customer of unavailable items.

3. **Generate Responses**:
   - Respond to product inquiries with relevant information from the product catalog.
   - Send confirmation or stock unavailability messages for order requests.

## Prerequisites
- Python 3.x
- Jupyter Notebook
- Libraries: Pandas, NumPy, Scikit-learn (or similar for ML tasks), NLTK/Spacy for natural language processing

## Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/retail-business-automation-system.git
    ```
2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```
3. Launch Jupyter Notebook:
    ```sh
    jupyter notebook
    ```

## Usage
1. Open the `Retail_Business_Automation_System.ipynb` notebook in Jupyter.
2. Follow the instructions in each section to execute the email processing and order management tasks.
3. Modify the product catalog or email dataset to test the system with different scenarios.

## Project Structure
- `Retail_Business_Automation_System.ipynb`: Main notebook containing the code for classification, order processing, and response generation.
- `data/`: Folder containing product data and email datasets.


## Dataset
- **Products**: Contains product details such as ID, name, category, stock amount, and descriptions.
- **Emails**: A collection of emails including ID, subject, and body.

## Enhancements
- The Responeses are not 100% accurate as there is a room of improvement.

