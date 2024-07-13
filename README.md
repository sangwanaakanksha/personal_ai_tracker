# personal_ai_tracker

Welcome to the Personal AI Tracker project! This tool leverages voice recordings, speech-to-text technology, and capabilities of Claude LLM to help you track and analyze your daily food intake, mood, and exercise routines.

## Features

- Transcribe voice recordings to text using the Google Cloud Speech-to-Text API
- Process transcriptions using the Anthropic Claude API to extract structured data and insights
- Categorize data into food, mood, and exercise tables with relevant columns
- Perform time series analysis and generate numeric insights
- Provide qualitative insights, trends, and suggestions based on collected data
- Store transcriptions and processed data for future reference and analysis
- Visualize the progress and analytics across tracked categories
  
## Current Version (v1)

The current version of the project includes the following components,

1. **Speech-to-Text**: Transcribe voice recordings stored in Google Cloud Storage using the Google Cloud Speech-to-Text API.
2. **Data Processing**: Process transcriptions using the Anthropic Claude API to extract structured data and insights across food, mood, and exercise categories.
3. **Data Storage**: Store transcriptions as text files and processed data in an Excel file. You can decide output format based on use case.
5. **Cost Tracking**: Track token usage and estimate the cost of API calls.

The project is currently functional and able to process voice recordings, extract insights, and store the results.

## Future Improvements (v2)

The current version is a good but limited starting point, there are several areas for improvement,

1. **Enhanced Data Processing**: Explore more advanced natural language processing techniques to extract more detailed and accurate insights from the transcriptions.
2. **Data Visualization**: Integrate data visualization tools to create interactive dashboards and charts for better data exploration and analysis.
3. **User Interface**: Develop a user-friendly interface to make it easier for users to upload voice recordings, view results, and interact with the tool.
4. **Data Persistence**: Implement a more robust data storage solution, such as a database, to store and manage the processed data effectively.
5. **Goal Tracking**: Add features to track and monitor progress towards specific goals, such as fitness targets or dietary improvements.

## Scaling the Idea

To scale the Personal AI Tracker project, following things to be considered, 

1. **Infrastructure**: Cloud services like Google Cloud Platform to handle increased data storage and processing needs.
2. **API Optimization**: Optimize the usage of the Speech-to-Text and Claude APIs to minimize costs and improve performance as the user base grows. For eg - if transcription already exists avoid sending duplicate calls to API
3. **Data Privacy and Security**: Implement strong data privacy and security measures to protect user data, including encryption, access controls, and secure communication protocols. By design, code uses regular expression to scrubb text off of PII, post which the text is shared with third party APIs.
5. **User Management**: Develop user authentication and authorization mechanisms to support multiple users and ensure data privacy.
6. **Integration**: Explore integrations with popular fitness tracking apps, nutrition databases, and other relevant services to enhance the functionality and value of the tool.

