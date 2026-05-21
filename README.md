# algorithmReview

# algorithmReview

The UML for this program, you should stick to this exact UML to make your program work.

+------------------------------------------------------------------+
|                            Restaurant                            |
+------------------------------------------------------------------+
| - name : String                                                  |
| - rating : double                                                |
| - menuItems : ArrayList<MenuItem>                                |
+------------------------------------------------------------------+
| + Restaurant()                                                   |
| + Restaurant(name : String, rating : double)                     |
| + getName() : String                                             |
| + setName(name : String) : void                                  |
| + getRating() : double                                           |
| + setRating(rating : double) : void                              |
| + getMenuItems() : ArrayList<MenuItem>                           |
| + setMenuItems(menuItems : ArrayList<MenuItem>) : void           |
| + addMenuItem(item : MenuItem) : void                            |
| + toString() : String                                            |
+------------------------------------------------------------------+

                    Restaurant HAS MANY MenuItems
Restaurant ------------------------------------------------> MenuItem



+------------------------------------------------------------------+
|                             MenuItem                             |
+------------------------------------------------------------------+
| - name : String                                                  |
| - description : String                                           |
| - price : double                                                 |
| - ingredients : ArrayList<Ingredient>                            |
+------------------------------------------------------------------+
| + MenuItem()                                                     |
| + MenuItem(name : String, description : String,                  |
|            price : double)                                       |
| + getName() : String                                             |
| + setName(name : String) : void                                  |
| + getDescription() : String                                      |
| + setDescription(description : String) : void                    |
| + getPrice() : double                                            |
| + setPrice(price : double) : void                                |
| + getIngredients() : ArrayList<Ingredient>                       |
| + setIngredients(ingredients : ArrayList<Ingredient>) : void     |
| + addIngredient(ingredient : Ingredient) : void                  |
| + toString() : String                                            |
+------------------------------------------------------------------+

                    MenuItem HAS MANY Ingredients
MenuItem ------------------------------------------------> Ingredient



+------------------------------------------------------------------+
|                            Ingredient                            |
+------------------------------------------------------------------+
| - name : String                                                  |
| - calories : int                                                 |
| - allergen : boolean                                             |
+------------------------------------------------------------------+
| + Ingredient()                                                   |
| + Ingredient(name : String, calories : int,                      |
|              allergen : boolean)                                 |
| + getName() : String                                             |
| + setName(name : String) : void                                  |
| + getCalories() : int                                            |
| + setCalories(calories : int) : void                             |
| + getAllergen() : boolean                                        |
| + setAllergen(allergen : boolean) : void                         |
| + toString() : String                                            |
+------------------------------------------------------------------+


+------------------------------------------------------------------+
|                        RestaurantSystem                          |
+------------------------------------------------------------------+
| + main(args : String[]) : void                                   |
| + loadRestaurants(filename : String)                             |
|       : ArrayList<Restaurant>                                    |
| + findRestaurant(restaurants : ArrayList<Restaurant>,            |
|                  name : String) : Restaurant                     |
| + printRestaurantReport(restaurants : ArrayList<Restaurant>)     |
|       : void                                                     |
| + getAveragePrice(restaurant : Restaurant) : double              |
| + getHighestPrice(restaurant : Restaurant) : double              |
| + getLowestPrice(restaurant : Restaurant) : double               |
| + getAverageCalories(restaurant : Restaurant) : double           |
+------------------------------------------------------------------+
