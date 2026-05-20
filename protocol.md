# TUESDAY 310326
Jacob Phillips 	
Buyer 	
	Unlimited Budget,
	4+ bathrooms or smaller house nearby, 
	big lot (tennis court & pool), 
	golf, 
	historic, 
	no waterfront
	
bathrooms  - more than 4 bathrooms
smaller house nearby - if sqft_living>sqft_living15
big lot - big sqft_lot 
historic - yr built
no waterfront - waterfront

SELECT id 
FROM king_county_house_details
WHERE 
	bathrooms >= 4,
	sqft_living>sqft_living15
	waterfront = 0,
ORDER BY
	sqft_lot,
	yr_built
	
 WATERFRONT HAS  ~2400 NAN

---

# WEDNESDAY 010426

How the number of bathrooms is related to the size of the living space

2
interpolate on sqft_basemenet and sqft_living for NaN


3
yrbuilt and yr renovated NAN

yrbuild and zipcode NAN

yrbuilt and lat and long NAN

create a boolean column renovated


-clean data
-interpolate or fill the NAN
-search for possible houses?

---

# THURSDAY 020426

1 Slide INTRO

-	EDA Project - Neue Fische - First Task - Date - Names

2 Slide WHO WE ARE
-	WE ARE H&A Real Estates - „Where Luxury Leaves Logic Behind.“
-	We catch your dream house while you sleep


3 Slide WHO IS THE CLIENT
-	Jacob is a weird and contradicting buyer
-	"Working with clients like Jacob Phillips requires us to look beyond the spreadsheet. 
	Their logic is not driven by market trends, but by personal myths. 
	We don't just sell square footage; we sell the space where their contradictions can coexist."

-	but one cannot truly understand the desires of a person without financial
	limitation. But who are we to judge.

4-5 Slide WHATS THE MARKET/ WHATS THE DATASET

- create 2 overview visualizations 

6 Slide HYPOTHESIS
-	1Hyp: House in lat/long that have a lot of space for pool&golf&tennis_court but with no waterfront
-	2Hyp: House with at least 4 bathrooms or small neighbor houses 
-	3Hyp: historic house but in great condition and not renovated (original)

7 Slide 1Hyp
-	### map lat/long, size points= size of sqft_lot
8 Slide 2Hyp
-	### bath symbol(size of the symbol = amount of bathrooms) vs small neighbor house(size of house symbol = mean of neighbor houses )  
9 Slide 3Hyp
-	### pie chart or box plot of different options

10 Slide CONCLUSION
-	list->#top10 of IDs from the database with the attributes 
map->. with attributes as symbols

-	extras -> top3 Recommendations (rating system)

11 Slide OUTRO
