# MedCompanion
Here's a README file for your Streamlit application with Plyer notifications:


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
#Output
![Screenshot 2024-06-19 072631](https://github.com/anushkas-11/MedCompanion/assets/123588192/db6808f3-ec45-42dc-b11e-67de2222bb12)
![Screenshot 2024-06-19 072652](https://github.com/anushkas-11/MedCompanion/assets/123588192/bf78f305-327b-42cb-ab5c-3520831ff961)
![Screenshot 2024-06-19 072711](https://github.com/anushkas-11/MedCompanion/assets/123588192/4b81d8cb-8879-4956-8511-dbe7dfaf2669)
![Screenshot 2024-06-19 072730](https://github.com/anushkas-11/MedCompanion/assets/123588192/b6c5851c-f343-42c9-9045-ad88f6bce0bf)
![Screenshot 2024-06-19 072757](https://github.com/anushkas-11/MedCompanion/assets/123588192/3e7abc05-1d1a-4d12-bed6-6cd4d596eb97)
![Screenshot 2024-06-19 072814](https://github.com/anushkas-11/MedCompanion/assets/123588192/46178235-9d0d-4af8-ad2a-cf73d5fae9c7)
![Screenshot 2024-06-19 072832](https://github.com/anushkas-11/MedCompanion/assets/123588192/a93a3688-3438-4cde-bc11-d58e953e5917)



## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.


---

### Contact

For any queries or issues, please contact [anushkasingh425@gmail.com].

---

Replace the placeholders like `your-username`, `your_pinecone_api_key`, `your_pinecone_environment`, and `your-email@example.com` with your actual details. Adjust the content as necessary to fit your specific application and requirements.

