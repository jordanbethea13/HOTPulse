# Hello Data Rockstar! 🌟

Welcome to your lab environment. 🧪

To make the most of this Hands on Training Session, please follow the exercises outlined in this lab manual. Each exercise is designed to help you apply what you've learned in a practical setting and gain valuable hands-on experience.

## Access Your Virtual Machine

To log into your VM, you will need to use the following credentials:

- **Username**: @lab.VirtualMachine(Win11-TC24).Username
- **Password**: @lab.VirtualMachine(Win11-TC24).Password

Once logged in you will find a link on the desktop to Tableau Online... Click the Icon:
<p align="center">
  <img src="https://i.ibb.co/SdvPnh0/Screenshot-2024-04-17-at-1-04-23-PM.png" alt="Tableau Cloud Login" width="25%" />
</p>

Tableau Cloud Credentials:

Username Email: **@lab.CloudCredential(TC2024-HOT1796).Username**

Password: **lab.CloudCredential(TC2024-HOT1796).Password**


Once you click into the Tableau Cloud Login shortcut you will be met with a login screen. Please enter your assigned username. 
<p align="center">
  <img src="https://i.ibb.co/JpMqY7g/tabcloudlogin2.png" alt="Tableau Cloud Login" width="50%" />
</p>

Once you enter the email into the first login you will be redirected to an Auth0 login screen.  Enter your username, and password into the fields...
<p align="center">
  <img src="https://i.ibb.co/8xm0gTb/auth0login.png" alt="Tableau Cloud Login" width="50%" />
</p>

Once done click continue and you will be signed into Tableau Cloud and you are ready for Exercise 1.  


<br>

# Exercise 1: Scavenger Hunt

## Background

As an emerging artist you have been focusing all of your energy into your passion and aspirations of playing in front of the largest crowds, preferably at **Data Fest**. However, it’s been a lot of time and effort trying to gain attention and visibility. One big area of mystery is who your fanbase is and what they’re resonating with. You decide to leverage **Tableau Pulse**. Pulse will help you make sense of the streaming data, social media engagement, and demographic data to set the foundation for data-driven decision making.

## Objective

Explore your artist data through **Tableau Pulse** to discover who your fans are and what resonates with them. Your findings will help shape your future marketing and engagement strategies.

## Instructions

Follow the clues provided below and use **Tableau Pulse** to uncover the answers. Keep track of your responses in this Google Form.

### Clue 1: Kickoff to Fan Engagement

- Where fans gather, the stars align. Begin where conversations ignite. Find the date when the spotlight began to shine.

### Clue 2: Rhythms of Streaming Success

- Streaming notes fill the air, from calm streams to tidal waves. Locate the metric where data unveils highs and lows. Which song made the numbers rave?

### Clue 3: Fanbase Footprint

- Fans tune in from far and near. From coast to coast, they hold you in their hearts so dear. Discover which state drums to the beat so you know which show you need to repeat.

### Clue 4: Social Media Symphony

- Across platforms wide, where do voices echo most? Seek the visual chorus of likes and shares' host. Which platform holds the crown, where fans' interactions boast? (Hint: you may need to follow two Pulse metrics)

### Clue 5: Trendsetter Tunes

- Trendsetters tune the public’s ear, making hits appear. Enter 'Trendsetter Track Triumph' and bring your findings here. Which track did influencers push, making its climb clear?

### BONUS: Curtain Call

- Summarize your findings and provide insights on how they can impact your strategy moving forward.

<br><br>
# Exercise 2: Create and Curate Pulse Metrics

### Important
This exercise cannot be completed until presenters have moved on past exercise 1.

## 🎵 Step into the Studio
Imagine stepping into the role of a visionary Music Producer, tasked with the thrilling challenge of crafting a groundbreaking EP alongside an Emerging Artist. In this bustling music industry, your mission is to create a unique sound that cuts through the noise and captures the hearts of listeners worldwide.

With **Tableau Pulse** at your fingertips, you have the power to dive deep into data-driven insights that inform every beat and note of your production. This isn't just about making music—it's about sculpting a sonic masterpiece that resonates on a personal level with your audience. You will:

Embrace your new role, harness the data, and start making musical history!
audience more efficiently.

## Quick Recap and Setup
- **We are giong to be Creating a new Pulse Metric** from a published Datasource on Tableau Cloud.
- **Project Folder where Data Source is located**: Same as your username (DataDazzler[x])
- **Data Source we will be using**: Music Production Details_[Your Username]
- **Note**: If you do not see the folder + Datasource, try refreshing the page.

## Steps to Create New Pulse Metric Definitions

1. **Verify Your Data Source**
   - Find your Datasource in the Project Folder and click into it.
   <p align="center">
  <img src="https://i.ibb.co/LZXPpJ9/ddfolder.png" alt="Tableau Cloud Login" width="90%" />
</p>
   - Verify that your datasource is in the folder with your username.
   <p align="center">
  <img src="https://i.ibb.co/xCY1sPj/datasourcecheck.png" alt="Tableau Cloud Login" width="75%" />
</p>
   - Click into **Tableau Pulse**.
  <p align="center">
  <img src="https://i.ibb.co/qn9VQ4B/datasourcecheck-V2.jpg" alt="Tableau Cloud Login" width="75%" />
</p>

2. **Create a New Metric Definition**
   - Click on “New Metric Definition”.
     <p align="center">
  <img src="https://i.ibb.co/CV850vd/CREATEMETRICdefinition.jpg" alt="Tableau Cloud Login" width="100%" />
</p>
   - Select the datasource from step 1b, search if needed.
    <p align="center">
  <img src="https://i.ibb.co/5rXrxrj/Select-Data-Source.jpg" alt="Tableau Cloud Login" width="100%" />
</p>
   - **Metric Definition Setup**:
     - **Name**: Spend
     - **Description**: The running total production spend across all artists.
     - **Value**: Spend
     - **Aggregation**: Sum
     - **Show Sparkline values to date as**: Running total
     - **Time dimension**: Date
     - **Compared to**: Leave as is
     - **Adjustable metrics filters**: Add all options: Artist Name, Campaign Type, Genre, Geographical Location, Listener Age Group, Listener Gender, Song Name
     <div style="display: flex; width: 100%;">
    <div style="width: calc(50% - 5px); padding-right: 5px;">
        <img src="https://i.ibb.co/YZ3VWy6/metriccreate.png" alt="Tableau Cloud Login" width="100%" />
    </div>
    <div style="width: calc(50% - 5px); padding-left: 5px;">
        <img src="https://i.ibb.co/X7YSQXJ/Metriccreate2.png" alt="Tableau Cloud Login" width="100%" />
    </div>
</div>
   - Click into the “Insights” tab.
    <p align="center">
  <img src="https://i.ibb.co/N7dmSDm/insights.jpg" alt="Tableau Cloud Login" width="50%" />
</p>
   - Change the option for ‘Value going up’ to “Unfavorable”.
    <p align="center">
  <img src="https://i.ibb.co/YPTHtf1/insights2.jpg" alt="Tableau Cloud Login" width="35%" />
</p>
   - Note Insight Types. If you would like to learn more about the insight types hover over the 'i' icon or visit our informational page on [Insight Types](https://help.tableau.com/current/api/rest_api/en-us/REST/rest_api_ref_pulse.htm#insight-types)

    <p align="center">
  <img src="https://i.ibb.co/ZfFtY8J/insights-3.png" alt="Tableau Cloud Login" width="35%" />
</p>
   - Click on **Save Definition**.

<br>
3. **Follow, Adjust, and Ask**
   - **Follow the Spend Metric**.
    <p align="center">
  <img src="https://i.ibb.co/prRsSjJ/follow.jpg" alt="Tableau Cloud Login" width="100%" />
</p>
   - Click **Breakdown**.
    <p align="center">
  <img src="https://i.ibb.co/3zwz28k/breakdown.jpg" alt="Tableau Cloud Login" width="100%" />
</p>
      - Notice the listener age group and analyze breakdown.
      - Click into Genre and analyze breakdown.
      - Click into Geographical Location and analyze breakdown.
   - **Ask Followup Questions**:
     - Click on “Which listener Age Group increased the most?” and take a look at the answer
      <p align="center">
  <img src="https://i.ibb.co/NVycMnw/question1.jpg" alt="Tableau Cloud Login" width="90%" />
</p>
     - Click on “Which Campaign Type decreased the most?” and check out the answer.
     - Click on “ASK” and type “Is there a new trend?”
      <p align="center">
  <img src="https://i.ibb.co/mDrrjyz/ask.jpg" alt="Tableau Cloud Login" width="90%" />
</p>
  
      - Feel free to click on a few additional generated questions if you would like.
   - **Create a Related Metric**:
     - Scroll to top and click on Adjust.
     <p align="center">
  <img src="https://i.ibb.co/jHjtPwK/adjust.jpg" alt="Tableau Cloud Login" width="100%" />
</p>
     - Click on **Week to Date”** and change to **“Year to Date”**.
     <p align="center">
  <img src="https://i.ibb.co/qs9mVb7/adjust2.jpg" alt="Tableau Cloud Login" width="40%" />
</p>
     - Click **blue checkmark** to make the adjustment.
     - Follow the new related metric you just created by clicking **"Follow"**.
     - Click back to “followed metrics”.

## Bonus
Create more metrics and keep exploring. Download counts, engagement rate, chart positions, playlist adds, reach, etc., can all have similar click paths with similar filters.

<br><br>
# Exercise 3: Publish Data Source and Pulse Metric

## 🎤 Welcome to Your New Gig as a Festival Planner!
You've rocked the music world by producing an EP, and now it's time to amp up your game as a Festival Planner! Dive into the vibrant and exhilarating world of music festivals, where you'll be the maestro behind the scenes. Armed with **Tableau Pulse**, you're set to masterfully coordinate sponsorship and ROI, handpick stellar artists, and craft marketing strategies that strike a chord with fans far and wide. 

## Publish a Data Source using Tableau Cloud
- Navigate back to **Tableau Cloud** from **Tableau Pulse**.
- Click **Explore**.
- Select **New > Published datasource**.
- Note all the options for connectors.
- Click on **"Files"**.
- Locate the data files in the desktop folder.
- Drag and drop or upload the file "Vendor Sponsor and ROI.csv" from the desktop folder.
- Click **File > Publish**.
- Publish your data into your **DataDazzler Folder** > Carrot dropdown to **"Exercise 3"**.

## Create a Metric from The Data Source
- Click back into **Tableau Pulse**.
- Click **"New Metric"**.
- Choose the **"Vendor Sponsor and ROI"** data source that you published into the Exercise 3 folder.
- Set up a new metric using what you learned from Exercise 2:
  - Choose a focus such as **Investment, ROI, or Sales/Engagement** - name the metric with your initials.
  - Add all filters, or have the audience choose.
- **Important**: Be sure to **Follow** any of the metrics you create. Many others will also be creating metrics, so it could get crowded at the moment. Name metrics with your initials to keep them organized.

### Note
This exercise requires careful attention to detail and understanding of data handling in Tableau. Make sure you follow the steps closely and use your new skills to enhance the festival planning process.

<br>
# 🌟 BONUS: Encore! Encore! Encore!

After you've completed the main exercises, take your data exploration to the next level. Dive deeper into the world of data and music festivals with this bonus challenge:

- **Explore More**: Use any of the datasources found in the folder on the desktop to continue creating metrics and pursuing your **"Data Fest"** goals.
- **Unleash Creativity**: Feel free to use any part of the platform to analyze and explore your data rockstar double life. Whether it’s adjusting filters, creating new metrics, or exploring different data visualizations, let your creativity guide you.
- **Share Insights**: If you discover something interesting, consider sharing it with your peers. Insightful findings can spark great conversations and lead to even more innovative ideas.

### 🎵 Let the Data Play
This is your chance to show off your skills and find insights that could illuminate your path as a data-driven festival planner. Enjoy the process, and let your inner data rockstar shine!