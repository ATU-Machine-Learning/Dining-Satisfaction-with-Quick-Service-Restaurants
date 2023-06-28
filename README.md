# Quick Service Restaurant Recommender
Given survey results on local Quick Service Restaurants (QSR) via the Dining Satisfaction with Quick Service Restaurants dataset, this project will guide through the development of a clustering-based recommendation system.

## Prerequisites
Programming experience in Python is recommended.
Some basic Data Science skills with Python are necessary, such as using Pandas, Numpy, and a visualization library (Matplotlib, Seaborn, etc.).

## Data Dictionary
* `Zip.code` - Participant's residential zipcode
* `Gender` - Participant's gender
    1. `1`: Male
    2. `2`: Female
    3. `3`: Other
* `Marital` - Participant's marital status
    1. `1`: Married
    2. `2`: Single
    3. `3`: Other
* `academic` - Participant's academic standing, if applicable
    1. `1`: Freshman
    2. `2`: Sophomore
    3. `3`: Junior
    4. `4`: Senior
    5. `5`: Graduate
    6. `6`: Other/Not A Student
* `Professional` - Participant's profession, if applicable
* `Age` - Participant's age group
    1. `1`: 18 to 24
    2. `2`: 25 to 34
    3. `3`: 35 to 44
    4. `4`: 45 to 54
    5. `5`: 55 to 64
    6. `6`: 65 or older
* `num.week` - How many times the participant visits a QSR in a week
* `num.month` - How many times the participant visits a QSR in a month
* `favorite.QSR` - A participant's favorite QSR
* `num.people` - How many people the participant lasted visited a QSR with

The following datapoints show how the participant heard about their last QSR visit, such as through a friend/relative or through social media:
* `friend.relative` - Participant heard about the QSR through a friend or relative
* `social.media` - Participant heard about the QSR through social media
* `flyer` - Participant heard about the QSR through a flyer
* `TV.ad` - Participant heard about the QSR through a television advertisement
* `News.ad` - Participant heard about the QSR through a newspaper/news segment advertisement
* `coupons` - Participant heard about the QSR through a coupon
* `billboard` - Participant heard about the QSR through a billboard
* `sign` - Participant heard about the QSR through a sign
* `drive` - Participant heard about the QSR through a drive-by
* `mobile` - Participant heard about the QSR through a mobile advertisement, such as a social media
* `other` - Participant heard about the QSR through another means

The following datapoints show the participant's preferences on their last QSR visit, rated 1 to 5, with 1 being the lowest and 5 being the highest:
* `appealing` - Participant found the QSR appealing
* `seat` - Participant found the QSR's seating available
* `parking` - Participant found the QSR's parking available
* `cleanliness` - Participant found the QSR's dining are to be cleanly
* `appearance` - Participant found the QSR's staff to be well-groomed and neat
* `friendliness` - Participant found the QSR's staff to be friendly and courteous
* `knowledge` - Participant found the QSR's staff to be knowledgeable
* `received` - Participant received their order correctly as ordered
* `billing` - Participant found the QSR's billing to be accurate
* `prompt` - Participant found the QSR's service to be prompt
* `attention` - Participant found the QSR's staff to be attentive
* `hours` - Participant found the QSR's operational hours to be convenient
* `waiting.time` - Participant found the QSR's waiting time to be reasonable
* `food.size` - Participant found the QSR's food portions to be reasonable
* `price` - Participant found the QSR's prices to be reasonable within comparison to other QSRs
* `wifi` - Participant found the QSR's WiFi to be available
* `Variety` - Participant found the QSR's drink and food menu to have a variety of options
* `value` - Participant found the QSR's food to be a good value
* `location` - Participant found the QSR's location to be convenient
* `drive.tru` - Participant found the QSR's drive-thru to be convenient and open
* `discounts` - Participant found the QSR's discounts to be available, including specials and coupons
* `health.food` - Participant found the QSR's food to be healthy, or at least have healthy options available
* `menu` - Participant found the QSR's menu to be easy to read and understand

The following datapoints show the participant's preferences on their last QSR visit, rated from Strongly Satisfied to Not Recommended, with 1 being the highest and 5 being the lowest:
* `last.visit` - Participant's overall satisfaction with their last QSR visit
* `visit.again` - Participant's likelihood to visit the QSR again
* `recommend` - Participant's likelihood to recommend the QSR to others, such as friends/relatives