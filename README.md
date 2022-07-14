# Software Engineering Job Application Bot (2.0) 👩🏾‍💻

A script to automatically search Glassdoor for job listings, aggregate every application URL, and apply to each job using pre-populated data. ***All with one click!***

![demo](https://user-images.githubusercontent.com/71213312/178988469-56eb68dc-32ad-4397-b227-d9668043b792.gif)

Ever sit at your desk for hours, clicking through endless job listings hoping to strike gold with one response? To solve this, I made a script a few months ago, which would take in a list of job URLs and automatically apply to potentially 100s of jobs with the click of a button. This was great, but there was one problem — the process of aggregating those links is painstaking. So, I wanted to automate that process with this project! ✨

__Installation__

1. Install [ChromeDriver](https://sites.google.com/a/chromium.org/chromedriver/) (or an alternatie driver for your browser of choice):
   * Run `brew cask install chromedriver`
   * Confirm installation: `chromedriver --version`
   * Check location of ChromeDriver: `which chromedriver`
   * Wherever the `driver` is initialized in the code, insert the ChromeDriver location
2. Install Selenium: `pip install selenium`(A tool designed for QA testing, but that actually works great for making these types of bots)
3. Install BeautifulSoup: `pip install beautifulsoup4`(A tool to scrape HTML/XML content (that saved be *big time* with this project)

__To test `get_links.py__

1. Uncomment the last line `get_links.py`
2. Run `$ python get_links.py`

__To run the entire script:__

1. Set a number of pages you'd like to iterate through here
2. Run `$ python apply.py`
3. The script will open [glassdoor.com](https://www.glassdoor.com/index.htm), at which point you should log-in
4. From there on, everything is automatic!

