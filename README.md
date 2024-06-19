# MedCompanion
Here's a README file for your Streamlit application with Plyer notifications:

---

# MedCompanion

MedCompanion is a Streamlit-based application designed to provide various health-related functionalities, including drug-drug interactions, drug-human interactions, medicine reminders, and an AI assistant for general queries. 

## Features

1. **Drug-Drug Interaction**: Check interactions between two drugs and understand their severity and descriptions.
2. **Drug-Human Interaction**: Analyze the potential interactions between a drug and a patient's medical history.
3. **Medicine Reminder**: Set reminders for taking medicines and receive notifications.
4. **AI Assistant**: Get answers to health-related questions using a language model.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/medcompanion.git
   cd medcompanion
   ```

2. **Create a virtual environment**:
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows, use `env\Scripts\activate`
   ```

3. **Install the dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up Pinecone API**:
   - Obtain your Pinecone API key and environment from [Pinecone](https://www.pinecone.io/).
   - Create a `.env` file in the project root and add your Pinecone credentials:
     ```
     PINECONE_API_KEY=your_pinecone_api_key
     PINECONE_API_ENV=your_pinecone_environment
     ```

5. **Prepare data files**:
   - Ensure you have the required CSV files (`chatbot.csv`, `ddi_dataset.csv`) in the project directory.

## Usage

Run the Streamlit app:

```bash
streamlit run app.py
```

### Tab Descriptions

1. **Drug-Drug Interaction**:
   - Enter the names of two drugs to check for potential interactions.
   - Displays the severity and description of the interaction.

2. **Drug-Human Interaction**:
   - Enter the drug being consumed and the patient's medical history.
   - Check for conditions like pregnancy, alcohol consumption, and breastfeeding.
   - Provides warnings based on the patient's medical conditions.

3. **Medicine Reminder**:
   - Enter the name of the medicine and the time to take it.
   - Sends a notification when it's time to take the medicine using Plyer.

4. **AI Assistant**:
   - Ask health-related questions.
   - Uses a language model to provide answers based on available information.

## Dependencies

- streamlit
- pandas
- requests
- plyer
- nltk
- langchain
- transformers
- pinecone-client

## Example

To set a medicine reminder:

1. Navigate to the "Medicine Reminder" tab.
2. Enter the name of the medicine.
3. Set the time for the reminder.
4. Click "Set Reminder".
5. A notification will be sent at the specified time.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.

---

### Contact

For any queries or issues, please contact [your-email@example.com].

---

Replace the placeholders like `your-username`, `your_pinecone_api_key`, `your_pinecone_environment`, and `your-email@example.com` with your actual details. Adjust the content as necessary to fit your specific application and requirements.
