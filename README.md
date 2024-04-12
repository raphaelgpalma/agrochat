## AgroChat 

<p align="center">
  <img src="https://github.com/raphaelgpalma/agrochat/blob/main/static/images/output.png" alt="Descrição da Imagem">
</p>


AgroChat is an innovative Django project that leverages real-time weather data to provide specific and efficient recommendations for each user. It integrates with the real-time weather data API to offer accurate information about current and future weather conditions. Moreover, it is enhanced with the ChatGPT generative text API, transforming it into an intelligent virtual assistant for agriculture.

## Prerequisites

Make sure to have the following requirements installed before getting started:

- **Python**: 
  - [Download Python](https://www.python.org/downloads/)

## Usage

1. Clone this repository:

```bash
git clone https://github.com/raphaelgpalma/agrochat.git
```

2. Virtual Environment Setup:

I recommend using a virtual environment to isolate project dependencies. Execute the following commands to create and activate a virtual environment:

```bash
# On Windows, use venv\Scripts\activate
# On Unix or MacOS, use source venv/bin/activate
python -m venv venv # Or virtualenv venv
source venv/bin/activate
```
3. Install Project Dependencies:

```bash
pip install -r requirements.txt
```

4. Create a .env file at the root of your project:

  ```bash
  touch .env
  ```

5. Using Docker to create the reverse proxy server
Ensure Docker is installed by referring to the Docker Installation Docs.
Run the following command:

```bash
docker run -dp 3040:3040 pawanosman/chatgpt:latest
```

Done! You can now connect to your local server's API at:

```bash
http://localhost:3040/v1/chat/completions
```

Note that the base URL is http://localhost:3040/v1

 5. Add on your .env file:

  ```bash
  OPEN_WEATHER_API_KEY=<YOUR OPEN WEATHER API KEY>
  ```

7. Run the Project's Server:

```bash
python manage.py runserver
```
If you want to stop running the server press CTRL+C on Terminal




   
