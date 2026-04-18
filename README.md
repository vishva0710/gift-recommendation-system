# gift-recommendation-system
A personalized gift recommendation system built using Machine Learning (Random Forest Classifier) that suggests the best gifts based on the receiver's personality, interests, relationship, occasion, and budget.
# Project Overview
Choosing the perfect gift is always challenging. This system solves that problem by taking simple inputs about the gift receiver and using a two-stage ML prediction pipeline to recommend the most suitable gift — first predicting the gift category, then the specific gift name.
# How It Works
User Inputs → Stage 1 Model → Top 4 Gift Types (with probability) → User Selects One → Stage 2 Model → Top 4 Specific Gift Names
Stage 1 — Gift Type Prediction
Predicts the best gift category from:
Accessory | Book | Electronics | Fashion Item | Grooming Set | Handmade Craft | Home Decor | Personalized Gift | Toy
Stage 2 — Gift Name Prediction
Based on the selected gift type, recommends specific gifts like:
Bluetooth Earbuds | Smart Watch | Fiction Novel | Customized Photo Frame | Skincare Kit | LED Table Lamp and 29 more options.
# Technologies Used
Python -->Core programming language
Pandas -->Data loading and preprocessing
NumPy  --> Numerical operations
Scikit-learn--> ML model (Random Forest), encoding, train-test split
Jupyter Notebook -->Development environment
# Data Preprocessing Steps
Removed unused features — user_id, age, small_business
Converted budget from numerical to categorical using pd.cut()
Applied multiple encoding strategies:
Binary Encoding → gender
One-Hot Encoding → occasion, receiver_personality, relationship_to_receiver, interests, giver_preference_style
Label Encoding → gift_type, gift_name
Ordinal Mapping → budget, receiver_age_group, relationship_closeness
# Input Features
Gender Male / Female
Age Group Child / Teen / Adult / Senior
Relationship Closeness distant / neutral / close / very close
Budgetbelow_500 / 500_to_1000 / 1000_to_3000 / 3000_to_5000
Occasion Birthday / Anniversary / Graduation / Farewell / Festival / Valentine's Day
Receiver Personality Creative / Emotional / Introvert / Extrovert / Practical
Relationship to Receiver Friend / Colleague / Teacher / Partner / Family
InterestsGaming / Home Decor / Fashion / Books / Tech / Travel / Art / Fitness / Music
Giver Preference Style practical / luxury / fun / sentimental
# Possible Gift Recommendations
The system can recommend from 35 unique gifts including:
Aroma Diffuser, Beard Grooming Kit, Bluetooth Earbuds, Bracelet, Cap, Clay Art Pot, Customized Keychain, Customized Photo Frame, Engraved Pen, Fiction Novel, Fitness Band, Handcrafted Candle, Handmade Greeting Card, LED Table Lamp, LEGO Set, Mini Indoor Plant, Motivational Book, Name Printed Mug, Neck Chain, Perfume Set, Portable Speaker, Puzzle Game, Remote Car, Scarf, Science Guide, Self-help Book, Skincare Kit, Sling Bag, Smart Watch, Soft Toy, Stylish T-shirt, Sunglasses, Wallet, Wall Art Frame, Wrist Watch












