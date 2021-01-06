# Developing operational strategy based on Linkedin Data
In this project I will try to determine the competition level in the staffing and recruiting sector based on data that I will scrape from the Linkedin platform.

## Web scraping using Selenium and Beautiful soup 
Firstly, I would like to say that the process is for educational reasons and with all respect to the LinkedIn platform and the companies. 

So, in this project we will work with Beautiful soup and Selenium libraries. In addition, it’s required to install a web driver, in my case I installed the final version of Chrome web driver. Notice that it's essential to find the driver that works with your current browser version, if you don’t know your Browser version you can download the last driver version and update your Browser. The last thing that you have to take care before jumping to the scrape part is to save the driver to a path that you can find easily. I saved the driver to the same folder with my coding files which is a solution that is not required to remember or search for a path.

After that step we are ready to open an editor, I used Jupyter notebook, a platform that you can print every step and I think for web scraping and in general is an amazing programming platform. Let’s start by importing the required libraries. 

![Χωρίς τίτλο](https://user-images.githubusercontent.com/66875726/103679154-2aae9680-4f8d-11eb-9a7b-3ae0584f8f10.png)

Now let’s open a browser using the web driver, I will work on Chrome platform but you can use whatever platform you prefer, notice that it’s essential to keep the  following window always open, this window will be the base of our next searching steps.

![Χωρίς τίτλο](https://user-images.githubusercontent.com/66875726/103694310-7704d100-4fa3-11eb-83ef-cfd2b881aa05.png)

Above is the base window, for reaching the LinkedIn web page we need a specific URL below is the URL and the code that I used.

![Χωρίς τίτλο](https://user-images.githubusercontent.com/66875726/103694779-322d6a00-4fa4-11eb-9127-50b88928d0af.png)

Running the code we are getting the following window where we should complete our personal information. In order to keep my personal information personal I created a txt file where I wrote in two lines my email and my password if you are not planning to share your code you can define two variables that will contain your personal information.


| Login page  | Submit     | 
| :---         |     :---:      |      
| ![Χωρίς τίτλο](https://user-images.githubusercontent.com/66875726/103699197-41fc7c80-4fab-11eb-8930-290f0d3e6fac.png)  |  ![1](https://user-images.githubusercontent.com/66875726/103698889-b8e54580-4faa-11eb-8b39-2bd02e6081b1.png) |

And here is the code that I used to login:



![Χωρίς τίτλο](https://user-images.githubusercontent.com/66875726/103701301-702f8b80-4fae-11eb-91be-7c7dd3ad281e.png)

So now we are in the initial LinkedIn page and we want to parse data based on a certain search. We could implement this step with different approaches, I think the easiest is to determine the link of the page that we are looking for, otherwise we have to use the Selenium library click in the search box determine our query after that we could also specify different filters in order to earn the information that we need. Definitely, using the direct link we avoid many lines of code.

![Χωρίς τίτλο](https://user-images.githubusercontent.com/66875726/103703411-31023a00-4fb0-11eb-8c0f-fe9cff784650.png)

So, the following code could be adjustable and everyone could be able to search for companies in specific sector’s. As I said, if you are interested in something else change the link and follow the next steps.

![Χωρίς τίτλο](https://user-images.githubusercontent.com/66875726/103704090-5e9bb300-4fb1-11eb-81a1-c1dcb03c23ba.png)

Notice that I used the Time Python module and the sleep command, don’t set aside this command and give some time to the browser to load the page in order to parse the page source code properly.

![Χωρίς τίτλο](https://user-images.githubusercontent.com/66875726/103704801-8d665900-4fb2-11eb-9f5c-b515455be378.png)

We are in the page that contains the information that we need to parse, in this step is necessary to know some html structure in order to inspect the elements that we need. For parsing elements I used the Beautiful soup library, we are in a static page now and we can detect the elements doing a left mouse click.

![Χωρίς τίτλο](https://user-images.githubusercontent.com/66875726/103705829-690b7c00-4fb4-11eb-907c-aee6c4bcf9b7.png)


