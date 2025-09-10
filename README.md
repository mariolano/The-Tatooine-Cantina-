# The Tatooine Cantina  

This repository contains a Python implementation of the **K-Nearest Neighbors (KNN)** algorithm in a *Star Wars*–themed scenario. The program predicts whether a new alien entering the Tatooine Cantina is **dangerous** or not, based on its similarity to known aliens.  

---

## Project Overview  
In this project, Han Solo records the traits of different aliens in the Tatooine Cantina, such as their **color, height, weight, and eyes**. When a new alien enters, the program uses the **KNN algorithm** to determine if it is dangerous.  

The project combines:  
- **Data preprocessing** (categorical → numeric values)  
- **Object-Oriented Programming in Python**  
- **Basic machine learning concepts** applied to a fun, narrative-driven scenario  

---

## What You’ll Learn  
By working with this repository, you will:  
- Understand and implement the **K-Nearest Neighbors (KNN)** algorithm from scratch.  
- Practice **Object-Oriented Programming (OOP)** principles in Python.  
- Learn how to use **Pandas** for reading and processing CSV datasets.  
- Explore how categorical data can be transformed into numeric coordinates.  
- Gain insight into **classification problems** and how predictions are made using majority voting.  

---

## Project Structure  

````markdown
tatooine-cantina/
│
├── TatooineCantina.py    # Main Python script with KNN class implementation
├── project_table.csv     # Dataset of aliens with attributes and "Dangerous" label
````

* **TatooineCantina.py**: Contains the `cantina` class (classify, distance, bubble sort, unpack, vote) and a `main()` function that runs the interactive program.
* **project\_table.csv**: Dataset of 8 aliens with attributes (Color, Height, Weight, Eyes in pairs, Dangerous).

---

## How It Works

1. **Dataset Load**

   * Alien traits are loaded from `project_table.csv` using **Pandas**.
   * The “Dangerous” column is separated for classification.

2. **Categorical → Numeric Conversion**

   * Traits (e.g., “Yellow”, “Tall”, “Pairs”) are converted into numbers via a dictionary.
   * Each alien becomes a tuple of numeric coordinates.

3. **User Input**

   * The user is prompted to enter a new alien’s attributes.
   * The value of **k** (number of neighbors) is chosen.

4. **KNN Algorithm**

   * Distances between the new alien and known aliens are calculated.
   * The closest **k neighbors** are found using a bubble sort.
   * A **majority vote** determines if the alien is “Dangerous” or “Not Dangerous.”

---

## Running the Program

Clone this repo and run:
```text
git clone https://github.com/your-username/tatooine-cantina.git
cd tatooine-cantina
python TatooineCantina.py
```

You’ll be prompted to enter:

The alien’s attributes in order: Color, Height, Weight, Eyes in pairs

The number of neighbors (k) to consider (1–8).

The program will then classify the alien as Dangerous or Not Dangerous.

## Start Demo

```text
Insert apparent alien attribute in the following order: Color(1), Height(2), Weight(3), and Eyes(4)
Make sure that you select an available variation of every attribute...

Insert variation of attribute (1) >>> Yellow
Insert variation of attribute (2) >>> Tall
Insert variation of attribute (3) >>> Normal
Insert variation of attribute (4) >>> Pairs

This is the alien to use for implementation >>> ['Yellow', 'Tall', 'Normal', 'Pairs']

Now choose the range k of neighbors to compare created alien with (max 8) >>> 3

Implementing KNN for new alien ['Yellow', 'Tall', 'Normal', 'Pairs'] with neighbor range 3...

New alien of classification (1, 3, 2, 2) is dangerous...
```

---

## Project Extension Ideas

Want to take this project further? Here are some ideas:

* **Larger Dataset**: Add more aliens to improve classification accuracy.
* **Visualization**: Use `matplotlib` to plot points and show neighbor distances.
* **Alternative Distance Metrics**: Try Manhattan or cosine distance instead of Euclidean.
* **Improve Sorting**: Replace bubble sort with a more efficient algorithm (e.g., quicksort).
* **Web Interface**: Build a simple Flask or Streamlit app to make the classifier interactive.
* **Apply to Real Data**: Replace aliens with another dataset (students, patients, customers).

---

## Maintainers & Contributors

* **Maria Olano**
* **Marc Jalkh**
* **Shrishti Thakur**

**(EECE 2140: Computing Fundamentals for Engineers)**
