# Problem Name: "Recipe Creation"

## Problem Statement:
You have information about `n` different recipes. You are given:
- A **string array `recipes`**, where `recipes[i]` represents the name of the `i`-th recipe.
- A **2D string array `ingredients`**, where `ingredients[i]` contains the list of ingredients required to create `recipes[i]`.
- A **string array `supplies`**, containing all the ingredients that you initially have (with infinite supply).

A **recipe can also be an ingredient** for other recipes, meaning `ingredients[i]` may contain a recipe from `recipes`.

### **Task**
Return a list of all the recipes that you can create, in any order.
### **Constraints**
- `n == recipes.length == ingredients.length`
- `1 <= n <= 100`
- `1 <= ingredients[i].length, supplies.length <= 100`
- `1 <= recipes[i].length, ingredients[i][j].length, supplies[k].length <= 10`
- `recipes[i]`, `ingredients[i][j]`, and `supplies[k]` consist only of lowercase English letters.
- All values in `recipes` and `supplies` are unique.
- Each `ingredients[i]` does not contain duplicate values.

---

### **Input Format**
- The first line contains an integer `n` - the number of recipes.
- The next `n` lines each contain a recipe name followed by its ingredients (space-separated).
- The next line contains an integer `m` - the number of supplies.
- The last line contains `m` space-separated strings representing the available supplies.

### **Output Format**
- A list of all the recipes that can be created.

---

### **Function Signature**
```python
def findAllRecipes(recipes: List[str], ingredients: List[List[str]], supplies: List[str]) -> List[str]: