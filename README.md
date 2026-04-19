# Neural Networks Projects
 
A collection of 6 neural networks projects completed as part of coursework.

---

## Project 1: Bike/Scooter Rental Demand Forecasting
 
**Task:** Predict the total number of bike/scooter rentals (`cnt`) per hour in a given city based on historical data.
 
**Dataset features:**
- Date and hour of rental
- Weather conditions (temperature, humidity, wind speed, weather situation)
- Day type (working day, holiday, weekday/weekend)

**Architecture (MLP):**
- 12 inputs
- 32 hidden neurons + ReLU
- 16 hidden neurons + ReLU
- 1 output

---

## Project 2

**Task:** Predict whether an apartment falls into the cheap (< 100 000$), average (100 000 - 350 000$) or expensive (> 350 000$) price category based on its attributes.

**Dataset features:**
- Building properties - year built, size in sqft, floor, hallway type, heating type, management type
- Parkings - number of ground and basement parking lots
- Public transport accessibility - time to bus stop, time to subway, nearest subway station
- Amenities and surroundings - number of elevators, managers, facilities inside/nearby, nearby school

**Architecture (MLP):**
- 33 inputs (after One-Hot Encoding)
- 64 hidden neurons + BatchNorm + ReLU
- 32 hidden neurons + BatchNorm + ReLU
- 3 outputs

---
 
## Project 3

**Task:** Classify images into one of 50 categories using a custom CNN architecture trained from scratch.

**Dataset:**
- ~90 000 labeled training images (64x64 RGB)
- 50 balanced classes

**Architecture (CNN):**
- 4 convolutional blocks (32 → 64 → 128 → 256 channels), each with 2x Conv2d + BatchNorm + GELU + MaxPool
- AdaptiveAvgPool (1x1)
- Dropout (0.5) + Linear classifier

**Training details:**
- AdamW optimizer with cosine annealing LR scheduler
- Data augmentation: random flip, crop, rotation, erasing
- Early stopping on validation loss

**Result: ~73% mean per-class accuracy**

---
 
## Project 4

---
 
## Project 5

---
 
## Project 6
