<a href="#">
  <div align="center">
    <img src="https://user-images.githubusercontent.com/30947706/79588950-17515780-80ee-11ea-8f66-e26da49fa052.png" width='154'/>
  </div>
</a>

<h1 align="center">Facebook Scraper (BETA)</h1>

<p align="center">
  Tooling that <b>automates</b> your social media interactions to collect posts, photos, videos, friends, followers and much more on Facebook.
</p>

<p align="center">
  <a href="https://awesomeopensource.com/project/harismuneer/Ultimate-Facebook-Scraper" target="_blank" rel="noopener noreferrer">
    <img src="https://user-images.githubusercontent.com/30947706/76143280-07c70380-6098-11ea-86b1-79fbce03888c.png" width="250" />
  </a>

<hr>

## News Updates 🏆
* 
* 

## Features 🚀

A bot which scrapes almost everything about a user's Facebook profile including:

- uploaded photos
- tagged photos
- videos
- friends list and their profile photos (including Followers, Following, Work Friends, College Friends etc)
- and all public posts/statuses available on the user's timeline
- **NEW:** Now you can scrape Facebook group posts.

Data is scraped in an organized format to be used for educational/research purposes by researchers. This scraper does not use Facebook's Graph API meaning there are no rate limiting issues.

**This tool is being used by thousands of developers weekly and we are pretty amazed at this response! Thank you!🎉**

For **citing/referencing** this tool for your research, check the 'Citation' section below.

## Note 🤝

This tool uses xpaths of **'divs'** to extract data. Since Facebook updates its site frequently, the 'divs' get changed. Consequently, we have to update the divs accordingly to correctly scrape data.

The developers of this tool have devoted time and effort in developing, and maintaining this tool for a long time. **In order to keep this amazing tool alive, we need support from you geeks.**

The code is intuitive and easy to understand, so you can update the relevant xpaths in the code if you find data is not being scraped from profiles. Facebook has most likely updated their site, so please generate a pull request. Much appreciated!

## Sample

<p align="middle">
  <img src="https://user-images.githubusercontent.com/30947706/79589043-34862600-80ee-11ea-9648-5ff86a63e464.png" width="700"/>
 </p>

## Screenshot

<p align="middle">
  <img src="https://user-images.githubusercontent.com/30947706/79589002-259f7380-80ee-11ea-959a-bddf0e2f6629.png" width="700"/>
 </p>

---

## Usage 🔧

### Installation 💻 

You will need to:

- Install latest version of [Google Chrome](https://www.google.com/chrome/).
- Install [Python 3](https://www.python.org/downloads/)
- Have a Facebook account without 2FA enabled

```bash
git clone https://github.com/xToxiCx-Team/Facebook-Scraper.git
cd Scraper-Facebook

# Install Python requirements
pip install -e .
```

The code is multi-platform and is tested on both Windows and Linux.
Chrome driver is automatically downloaded using the chromedriver_manager package.

### How to Run

- Fill your Facebook credentials into [`credentials.yaml`](credentials.yaml)
- Edit the [`input.txt`](input.txt) file and add profile, groups and individual group posts links as you want in the following format with each link on a new line:

Make sure the link only contains the username or id number at the end and not any other stuff. Make sure its in the format mentioned above.

Run the `Facebook-Scraper` command ! 🚀

```python
python scraper/scraper.py
```

> Note: There are two modes to download Friends Profile Pics and the user's Photos: Large Size and Small Size. By default they are set to Small Sized Pics because its really quick while Large Size Mode takes time depending on the number of pictures to download.

You can personalize your scrapping needs using the command line arguments:

```python
python scraper/scraper.py \
    --uploaded_photos True \
    --friends_photos True \
    --friends_small_size True \
    --photos_small_size True \
    --total_scrolls 2500 \
    --scroll_time 8
```

Note that those are the default values so no need to write them down if you're just testing or are okay with them.


---

## Important Message ⚠️

This tool is for research purposes only. Hence, the developers of this tool won't be responsible for any misuse of data collected using this tool. Used by many researchers and open source intelligence (OSINT) analysts.

This tool will not works if your account was set up with 2FA. You must disable it before using.

---

## Authors 👋

You can get in touch with us on our Facebook Profile:

#### [Michael Magdy](https://www.facebook.com/xToxiCx.Team/)

If you liked the repo then please support it by giving it a star ⭐!

## For Future 🔮

There are a lot of features that can be added to this tool like adding support for pages, groups, comments etc! Please contribute :)

## Contributions Welcome ✨

![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)

If you find any bug in the code or have any improvements in mind then feel free to generate a pull request.

> Note: We use [Black](https://pypi.org/project/black/) to lint Python files. Please use it in order to have a valid pull request 😉

## Issues 🔨

[![GitHub Issues](https://img.shields.io/github/issues/harismuneer/Ultimate-Facebook-Scraper.svg?style=flat&label=Issues&maxAge=2592000)](https://github.com/xToxiCx-Team/Facebook-Scraper/issues)

If you face any issue, you can create a new issue in the Issues Tab and I will be glad to help you out.

## License 📄

[![MIT](https://img.shields.io/cocoapods/l/AFNetworking.svg?style=style&label=License&maxAge=2592000)](LICENSE)

Copyright (c) 2020 xToxiCx
