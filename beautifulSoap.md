#IMPORT RESOURCES import requests from bs4 import BeautifulSoup

#MAKE A SOAP OBJECT OUT OF A WEBSITE // 1. The HTTP request webpage = request.get('URL', 'html.parser'); // 2. Turn the website into a soup object soup = BeautifulSoup(webpage.content);

#OBJECT TYPES //1. Tags correspond to HTML tags Example Code: soup = BeautifulSoup('

An example div
An example p tag

');
print(soup.div); -->

An example div
--> gets the first tag of that type on the page
print(soup.div.name) print(soup.div.attrs) --> div --> {'id': 'example'}

//2. Navigable Strings: Piece of text inside of HTML Tags print(soup.div.string) --> An example div

#NAVIGATING BY TAGS Example Code:

World's Best Chocolate Chip Cookies
Ingredients
1 cup flour
1/2 cup sugar
2 tbsp oil
1/2 tsp baking soda
½ cup chocolate chips
1/2 tsp vanilla
2 tbsp milk
//1. Get the children of a tag: for child in soup.ul.children: print(child) -->

1 cup flour
-->
1/2 cup sugar
...
//2. Get the parent of a tag: for parent in soup.li.parents: print(parent)

#FIND ALL //1. find_all() print(soup.find_all("h1")) --> Outputs all

...
on the website
//1.1. find_all() with regex import re soup.find_all(re.compile("[ou]l")) --> Outputs all

...
and
...
soup.find_all(re.compile("h[1-9]")) --> Outputs all headings
//1.2. find_all() with lists soup.find_all(['h1', 'a', 'p'])

//1.3 find_all() with attributes soup.find_all(attrs={'class':'banner', 'id':'jumbotron'});

//1.4 find_all() with functions def has_banner_class_and_hello_world(tag): return tag.attr('class') == "banner" and tag.string == "Hello world"

soup.find_all(has_banner_class_and_hello_world)

#CSS SELECTORS //1. grab CSS classes with .select("class_name") soup.select(".recipeLink")

//*2. grab CSS IDs with .select("#id_name") soup.select("#selected")

//3. using a loop for link in soup.select(".recipeLink > a"): webpage = requests.get(link) new_soup = BeautifulSoup(webpage)
