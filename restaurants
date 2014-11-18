"""
Here are some example dictionaries. These correspond to the information in
restaurants_small.txt
Restaurant name to rating:
#dict of {str: int}
name_to_rating = {'Georgie Porgie': 87,
'Queen St. Cafe': 82,
'Dumplings R Us': 71,
'Mexican Grill': 85,
'Deep Fried Everything': 52}

Price to list of restaurant names:
#dict of {str: list of str}
price_to names{'$': ['Queen St. Cafe', 'Dumplings R Us', 'Deep Fried Everything'],
'$$': ['Mexican Grill'],
'$$$': ['Georgie Porgie'],
'$$$':[]}

Cuisine to list of restaurant names:
#dict of {str: list of str}
cuisine_to_names = {'Canadian': ['Georgie Porgie'],
'Pub Food': ['Georgie Porgie', 'Deep Fried Everything'],
'Malaysian': ['Queen St. Cafe'],
'Thai': ['Queen St. Cafe'],
'Chinese': ['Dumplings R Us'],
'Mexican': ['Mexican Grill']}

With this data? for a price of '$' and cuisines of ['Chinese', 'Thai'] we
would produce this list:
    [[82, 'Queen St.Cafe'], [71, 'Dumpings R Us']]
"""
# The file containing the restaurant data.
FILENAME = 'restaurants_small.txt'
read_restaurant()
def recommend(file, price, cuisines_list):
    """(file open for reading, str, list of str) -> list of [int, str] list

    Find restaurants in fole that are priced according to price and that are
    tagged with any of the items in cuisines_list. Return a list of lists of
    the form [rating%, restaunat name], sorted by rating%.
    """

    #Read the file and build the data structures.
    # - a dict of {restaurant name: rating%}
    # - a dict of {price: list of restaurant names}
    # - a dict of {cuisine: list of restaurant names}
    name_to_rating, price_to_names, cuisine_to_name = read_restaurants()

    #Look for price or cuisines first?

    #Price: look up the list of restaurant names for the requested price.

    #Now we have a list of restaurans in the rigth price range.
    #Need a new list of restaurants that serve one of the cuisines.

    #Now we have a list of restaurants that are in the right price range and serve
    #the requested cuisines
    #Need to look at ratings and sort this list.

    #We're done! Return the sorted list.
def read_restaurant():
    """(file) - (dict, dict, dict)

    Return a tuple of three dictionaries basedon the information in the file:
     - a dict of {restaurant name: rating%}
     - a dict of {price: list of restaurant names}
     - a dict of {cuisine: list of restaurant names}
     """
    name_to_rating = {}
    #price_to_names = {'$': [], '$$': [], '$$$': [], '$$$$': []}
    #cuisine_to_names = {}
    file = "restaurants_small.txt"
    y = open(file, 'r').read()
    exec(y)
    y.close()
    
    return name_to_rating#, price_to_names, cuisine_to_names
