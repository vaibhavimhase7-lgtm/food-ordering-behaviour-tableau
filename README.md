# Food Ordering Behaviour and Consumer Trends: A Structured Analysis of Choices and Habits

A data analytics project built with **Tableau**, with the dashboard and story embedded in a **Flask** web application. It was created as part of the Data Analytics with Tableau program on SkillWallet (SmartBridge).


## Project Overview

Food delivery platforms collect a large amount of data about what people order, when they order, and how they rate their meals. This project analyses that data to understand customer choices and ordering habits, and presents the findings as interactive visualizations that restaurants, delivery platforms, and decision-makers can use.

## Objectives

- Understand which cuisines and meal types are most popular
- Compare ordering behaviour across cities and age groups
- Study delivery time, order value, and customer ratings
- Present the insights through an interactive dashboard and a data story
- Make the analysis accessible in a browser through a Flask website

## Dataset

- **File:** `food_ordering_behavior_dataset.csv`
- **Size:** 50,000 rows and 21 fields
- **Cities covered:** Bangalore, Chandigarh, Delhi, Hyderabad, Mumbai, Pune
- **Example fields:** Order ID, User ID, Age, City, Cuisine, Meal Type, Restaurant Type, Delivery Fee, Delivery Time, Customer Rating

## Tools and Technologies

| Tool | Purpose |
|------|---------|
| Tableau Desktop / Tableau Public | Data preparation, visualization, dashboard, story |
| Python 3 | Backend language |
| Flask | Web application to embed the dashboard and story |
| HTML, CSS | Website pages and styling |
| GitHub | Version control and project hosting |

## Visualizations

The dashboard includes these views:

- City vs Cuisine (heat map)
- Orders by Age Group and Restaurant Type
- Cuisine Preference Distribution
- Company Type and Meal Type Orders
- Meal Type vs Customer Rating
- Top 5 Cities by Order Volume
- Order Intelligence: Cuisine, Timing and Spend
- Delivery Time Distribution

The **story** combines these views into a step-by-step narrative of the key findings.

## Project Structure

```
food-ordering-behaviour-tableau/
├── app.py                  # Flask application
├── templates/
│   └── index.html          # Website page with embedded Tableau dashboard and story
├── static/                 # CSS, images, and other static files
├── data/
│   └── food_ordering_behavior_dataset.csv
├── tableau/
│   └── FOOD ORDERING BEHAVIOUR.twbx
├── screenshots/            # Dashboard, story, and website screenshots
└── README.md
```

## Project Workflow

1. **Data Collection and Extraction:** loaded the CSV dataset into Tableau
2. **Data Preparation:** checked and cleaned the fields
3. **Data Visualization:** created charts and sheets
4. **Dashboard:** combined the sheets into one interactive dashboard
5. **Story:** built a narrative from the key insights
6. **Performance Testing:** checked that filters and views load correctly
7. **Web Integration:** published to Tableau Public and embedded in Flask
8. **Documentation and Demonstration:** recorded a demo and wrote this README

## How to Run the Project

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/food-ordering-behaviour-tableau.git
   cd food-ordering-behaviour-tableau
   ```

2. **Install Flask**
   ```bash
   pip install flask
   ```

3. **Run the application**
   ```bash
   python app.py
   ```

4. **Open in your browser**
   ```
   http://127.0.0.1:5000
   ```

## Flask Code

```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def home():
    return render_template("index.html")

if __name__ == '__main__':
    app.run(debug=True)
```

## Screenshots
```
![Dashboard](<img width="1605" height="842" alt="Screenshot 2026-10-07 075645" src="https://github.com/user-attachments/assets/0c0963ec-4e4b-42f9-80d8-2d8bd6a67c65" />
)(<img width="1602" height="838" alt="Screenshot 2026-10-07 075710" src="https://github.com/user-attachments/assets/9a30b14a-5069-4154-9bb3-4ddeef0b8474" />
)
![Story](<img width="1656" height="848" alt="Screenshot 2026-10-07 075923" src="https://github.com/user-attachments/assets/b48e6a14-52a1-4ae7-a426-2da4d7d41f49" />
)
![Website](https://public.tableau.com/views/FOODORDERINGBEHAVIOUR_twbx/FOODORDERINGBEHAVIOURSTORY?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
```

## Key Insights

## Key Insights

- **Most popular cuisine:** DESERTS has the highest share of orders in Mumbai.
- **Top city:** Mumbai has the highest order volume with 1463 orders.
- **Most active age group:** youngsters places the most orders.
- **Meal type and rating:** breakfast receives the highest average customer rating.
- **Delivery time:** most orders are delivered in about avg 7.4 minutes.

## Author

**VAIBHAVI MHASE**
vaibhavimhase7@gmail.com

## Acknowledgements

- SkillWallet, a SmartBridge product
- Tableau Public for hosting the dashboard and story
