# Weather Chatbot Assistant

## Overview

This project is a chatbot assistant that provides real-time weather updates and forecasts. It integrates external APIs for weather data and employs reasoning techniques such as Chain of Thought (CoT) and ReAct to enhance its responses.

## Features

- **Weather Data Retrieval**: Get current weather conditions and multi-day forecasts.
- **Stepwise Query Breakdown**: Uses logical reasoning to handle complex weather-related questions.
- **Iterative Decision-Making**: Implements Thought → Action → Observation for improved accuracy.

## Installation

### Clone the Repository

```sh
git clone https://github.com/your-username/weather-chatbot.git
cd weather-chatbot
```

### Install Dependencies

```sh
pip install openai python-dotenv requests
```

### Setup API Keys

Create a `.env` file and add your API keys:

```sh
OPENAI_API_KEY=your_openai_api_key
WEATHER_API_KEY=your_weatherapi_key
```

### Running the Chatbot

```sh
python chatbot.py
```

## Example Interactions

### **Simple Weather Query**

**User**: What's the weather in Berlin?

**Bot**: The current temperature in Berlin is 12°C with partly cloudy skies.

### **Comparing Weather Conditions**

**User**: How does the weather in Miami compare to Los Angeles?

**Bot**:

- Miami: 28°C, humid
- Los Angeles: 22°C, sunny
- Miami is warmer and more humid than Los Angeles.

### **Reasoning Through a Query**

**User**: Should I carry an umbrella in Tokyo tomorrow?

**Bot**:

**Thought**: Check the weather forecast for Tokyo tomorrow.
**Action**: [Retrieves Tokyo's weather forecast]
**Observation**: 80% chance of rain.
**Final Answer**: Yes, you should carry an umbrella as rain is highly likely.

## Challenges Faced

- **API Management**: Ensuring secure storage and retrieval of API keys.
- **Error Handling**: Providing fallback responses when API data is unavailable.
- **Enhanced Reasoning**: Improving chatbot accuracy using structured decision-making.

## Resources

- [OpenAI API Documentation](https://platform.openai.com/docs)
- [WeatherAPI Documentation](https://www.weatherapi.com/docs/)

