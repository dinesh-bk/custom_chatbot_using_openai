# **Custom Chatbot using OpenAI**

Welcome to the **Build Your Own Custom Chatbot** project! This repository contains the code and resources to create a custom chatbot powered by OpenAI. You will use various datasets to customize the chatbot to respond to specific domains or scenarios.

## **Project Overview**
In this project, you'll customize an OpenAI chatbot by integrating it with a dataset of your choice. The goal is to demonstrate how the chatbot's behavior can be tailored by using a custom data source to answer domain-specific questions.

### **What Will You Build?**
By the end of this project, you will have a fully functional chatbot trained on custom data to answer questions in a specific scenario. You will:
- Select and integrate a data source.
- Explain why your chosen data source is appropriate for the chatbot’s task.
- Implement the integration of the data source into the chatbot’s code.
- Design questions to test the chatbot’s performance with and without the custom data.

## **Getting Started**

### **Prerequisites**
Before running the project, ensure you have the following tools installed:
- Python 3.x
- OpenAI Python SDK
- pandas
- requests (for using APIs such as Wikipedia)

### **Installation**
Clone this repository to your local machine:

```bash
git clone https://github.com/yourusername/custom-chatbot.git
cd custom-chatbot
```

Install the required packages:

```bash
pip install -r requirements.txt
```

### **Data Sources**
There are two main types of data sources that can be used in this project:
1. **Wikipedia API**: Ideal for fetching articles from Wikipedia, similar to the examples used in demo exercises.
2. **CSV Files**: This project provides several CSV files in the `data/` directory that can be used for training the chatbot:
   - `2023_fashion_trends.csv`: Contains information on fashion trends for 2023.
   - `character_descriptions.csv`: Contains fictional character descriptions from theater, television, and film.
   - `nyc_food_scrap_drop_off_sites.csv`: Lists NYC food scrap drop-off sites and their details.

Alternatively, you can use your own data by sourcing or scraping other text-based data (must have at least 20 rows).

### **Custom Scenario**
The customization involves:
1. **Dataset Selection**: Choose a dataset relevant to your scenario. You can explain why this dataset is appropriate for the chatbot's tasks. For example:
   - *Using the `2023_fashion_trends.csv` to build a chatbot that answers questions about the latest fashion trends.*
2. **Custom Integration**: Integrate the dataset into the chatbot’s code and test the performance of the chatbot before and after customization.
3. **Demonstration**: At the end of the project, demonstrate how the chatbot performs in answering questions with and without the custom data. This helps highlight the effectiveness of your chosen data.

## **How to Use the Chatbot**

1. **Step 1**: Load the data source you want to integrate with the chatbot.
2. **Step 2**: Modify the chatbot’s code to leverage the dataset.
3. **Step 3**: Ask questions using the chatbot and observe how the answers differ based on the integration of the custom data.

### **Running the Chatbot**

- To run the chatbot, launch the provided notebook (`project.ipynb`) and follow the steps:
  1. Load your dataset.
  2. Initialize the chatbot.
  3. Ask questions in the before and after customization sections.

### **Example Usage**

```python
# Example of chatbot before customization
question = "What are the latest fashion trends?"
response = chatbot.ask(question)
print(response)

# Customizing with '2023_fashion_trends.csv'
custom_chatbot = CustomChatbot("data/2023_fashion_trends.csv")
response = custom_chatbot.ask(question)
print(response)
```

## **Evaluation**
- At the end of the notebook, there is a **Q&A comparison** section where you can test the chatbot’s performance with and without customization to observe the changes in responses.

## **Data Considerations**
When selecting or creating your dataset:
- Ensure that it contains at least 20 rows.
- Focus on text-based data, as OpenAI models are optimized for handling natural language rather than numerical or logical data (e.g., budgets, inventory).

## **Files and Directories**

- `project.ipynb`: The main Jupyter notebook where you will implement and customize the chatbot.
- `data/`: This directory contains the CSV files available for use in the project.
- `requirements.txt`: The list of Python packages needed to run the project.

## **Contributing**
Contributions are welcome! Please create a pull request if you have any improvements or additional features to propose.
