# Developing operational strategy based on Linkedin Data
In this project I will try to determine the competition level in the staffing and recruiting sector based on data that I will scrape from the Linkedin platform.

## Web scraping using Selenium and Beautiful soup 
Firstly, I would like to say that the process is for educational reasons and with all respect to the LinkedIn platform and the companies. 

So, in this project we will work with Beautiful soup and Selenium libraries. In addition, it’s required to install a web driver, in my case I installed the final version of Chrome web driver. Notice that it's essential to find the driver that works with your current browser version, if you don’t know your Browser version you can download the last driver version and update your Browser. The last thing that you have to take care before jumping to the scrape part is to save the driver to a path that you can find easily. I saved the driver to the same folder with my coding files which is a solution that is not required to remember or search for a path.

After that step we are ready to open an editor, I used Jupyter notebook, a platform that you can print every step and I think for web scraping and in general is an amazing programming platform. Let’s start by importing the required libraries. 

![Χωρίς τίτλο](https://user-images.githubusercontent.com/66875726/103679154-2aae9680-4f8d-11eb-9a7b-3ae0584f8f10.png)

Now let’s open a browser using the web driver, I will work on Chrome platform but you can use whatever platform you prefer, notice that it’s essential to keep the  following window always open, this window will be the base of our next searching steps.

![Χωρίς τίτλο](https://user-images.githubusercontent.com/66875726/103686182-196a8780-4f97-11eb-8864-a31d2e4c36d6.png)

Above is the base window, for reaching the LinkedIn web page we need a specific URL below is the URL and the code that I used.

