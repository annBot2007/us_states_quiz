# us_states_quiz
Geography Quiz Time!

This project is a **graphical quiz game** built using Python that challenges the player to **name all 50 U.S. states**. As the player types correct answers, the corresponding state names are displayed **on a map of the United States**.

**Features:**

#### 1. **Interactive Game Interface**

Utilizes the **`turtle` graphics library** to display a **blank U.S. map** image. Players interact with the game by typing state names into popup input boxes, and correct guesses are written directly onto the map using turtle’s `write()` method.

#### 2. **Use of CSV Files**

The project uses a **CSV file (`50_states.csv`)** which contains:

* The names of all 50 states
* Their **(x, y)** coordinates for accurate placement on the map

This data file is essential for checking answers and positioning state names correctly on the turtle screen.

#### 3. **Use of `pandas` Library**

The **`pandas`** library is used to:

* Load and read the CSV file into a `DataFrame`
* Easily access and filter the list of states
* Compare user input with the correct answers
* Track which states have already been guessed

---

### **How It Works:**

* The game starts with a blank map of the U.S.
* The player is prompted to guess a state name.
* If the guess is correct and hasn't been guessed before:
  * The name is written on the map at the correct coordinates.
  * The score increases by 1.
* If the guess is incorrect or already guessed:
  * The player is notified but the score remains unchanged.
* The game continues until all 50 states are correctly identified or the user exits.


### **Skills Demonstrated:**

* Reading and manipulating CSV data using `pandas`
* Drawing and text placement with `turtle`
* Conditional logic and loops
* Real-time user interaction with `screen.textinput()`
* Tracking progress with variables and DataFrame operations
