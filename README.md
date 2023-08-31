# YouTube  Analysis
 This repository contains a data analysis project that showcases how to retrieve data from the YouTube API, clean and analyze the data using Python, and create visualizations using various data analysis libraries. 
 ## Project Overview 
 The project demonstrates the following steps:
  - Fetching data from the YouTube API using the `googleapiclient` library.
  - Cleaning and preprocessing the data using the `pandas` and `emoji` library. 
  - Performing data analysis and visualization using `seaborn` and `matplotlib`. 
  - Creating insightful visuals and drawing conclusions from the data. 
  
 ## Getting Started
  ### Prerequisites
 Before you begin, make sure you have the following prerequisites: 
  - Python 3.x 
  - Jupyter Notebook (inside VS Code or any other environment)
  - Install all necessary libraries using `pip install` command
  
   Clone the repository:
    ```bash git clone https://github.com/your-username/YouTube_Analysis.git cd YouTube_Analysis ```
   
## How to get Youtube Developer Key for API
To run the project, you'll need a YouTube API key. Follow these steps to obtain your API key:
*  Go to the Google Cloud Console ("https://console.cloud.google.com/").
* Create a new project.
*  Enable the YouTube Data API v3 for your project. 
* Create credentials and select  "API Key".
*  Copy the generated API key.


## Using the .env File to Secure Your API Key 
The .env file is used to store sensitive data like API keys. It is not included in version control and keeps your sensitive information private. To use the .env file to store your YouTube API key:   

*  Create an .env file in the project directory. 
* Add the following line to the .env file: 
	* ```python YOUTUBE_API_KEY=your_api_key_here ``` 
* Replace your_api_key_here with the API key you obtained. 
* Load the API key in your Python script using python-dotenv: 
	* ```python
		from dotenv import load_dotenv
		# Load the API key from .env file 
		load_dotenv() 
		# Access the API key from  .env file
		api_key = os.getenv('YOUTUBE_API_KEY')
	```



# Finding Channel ID on YouTube

To find the Channel ID of a YouTube channel, you can follow these steps:

1. Open a web browser and go to YouTube (https://www.youtube.com).
2. Search for the channel whose ID you want to find.
3. Click on the channel's name to open their profile page.
4. Look at the URL in the address bar of the browser. It should look something like this:
	[https://www.youtube.com/channel/ChannelIDHere](https://www.youtube.com/channel/ChannelIDHere)
 

If the channel name appears instead of the channel id, perform the following steps:
1. Open the channel's profile page by clicking on its name. <br />
  ![Screenshot (587)](https://github.com/Chirag529/Youtube_Analysis/assets/87868888/c8bbb42b-82d3-4b34-8d7e-7843e3202fd7)
 <br />

2. Right-click and select View Page Source (or press CTRL + U). <br />
   ![view page source](https://github.com/Chirag529/Youtube_Analysis/assets/87868888/11fe2494-a733-4f23-8108-086ec4847959)
  <br />
  
3. Next, press CTRL + F to search the page. <br />
   ![Screenshot (589)](https://github.com/Chirag529/Youtube_Analysis/assets/87868888/3f32b836-b5ee-4767-89d1-8406381b247c)
   <br />
   
4. Enter "channel" there and click enter. <br />
  ![Screenshot (590)](https://github.com/Chirag529/Youtube_Analysis/assets/87868888/4aac54c2-6c40-413d-881a-3bb251c8d09e)
   <br />
   
6. There will be one link containing the channel id; copy it from there. <br />
  ![Screenshot (590)](https://github.com/Chirag529/Youtube_Analysis/assets/87868888/8140c72d-0bc0-48ea-8910-7271152b38f2)
  <br />
