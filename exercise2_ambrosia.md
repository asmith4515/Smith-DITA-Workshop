# Exercise 2: Ambrosia Salad Recipe

## Genre Analysis

If someone wants to cook a dish or bake a dessert they are not able to remember, they will often turn to a recipe or an instructional guide. In this case, a recipe can be seen as an instructional genre. The person who created the recipe then becomes the author who is passing down their knowledge, and the reader is the person who is learning from the recipe. The information within the recipe is very helpful and insightful because it includes things such as the ingredient/shopping list, the mandatory steps, and lastly the completed dish or dessert. I specifically chose this recipe because ambrosia salad is simple and easy. 

The recipe itself has three genre sections which are the title, the ingredients, and the steps needed to put it all together. The ingredients can be broken down into quantities, units, items, and even preparation notes for certain ingredients (using words such as "drained"). In order to assemble the genre sections and elements, you have to be consistent with the organization. For instance, titles always come first, the ingredient list should come after the title but before the steps are given, and finally, the steps should be placed in order to avoid any mistakes or confusion.

## DTD File

```

<!ELEMENT recipe (title, ingredients, directions)>
<!ELEMENT title (#PCDATA)>
<!ELEMENT ingredients (ingredient+)>
<!ELEMENT ingredient (quantity, unit*, item, preparation*)>
<!ELEMENT quantity (#PCDATA)>
<!ELEMENT unit (#PCDATA)>
<!ELEMENT item (#PCDATA)>
<!ELEMENT preparation (#PCDATA)>
<!ELEMENT directions (step+)>
<!ELEMENT step (#PCDATA)>
```

## XML File

```

<!DOCTYPE recipe SYSTEM "ambrosia.dtd">
<recipe>
<title>Ambrosia Salad</title>
<ingredients>
<ingredient>
<quantity>1</quantity>
<unit>can (11 oz.)</unit>
<item>mandarin oranges</item>
<preparation>drained</preparation>
</ingredient>
<ingredient>
<quantity>1</quantity>
<unit>can (20 oz.)</unit>
<item>pineapple tidbits</item>
<preparation>drained</preparation>
</ingredient>
<ingredient>
<quantity>1</quantity>
<unit>c.</unit>
<item>mini marshmallows</item>
</ingredient>
<ingredient>
<quantity>1</quantity>
<unit>c.</unit>
<item>shredded coconut</item>
</ingredient>
<ingredient>
<quantity>1/2</quantity>
<unit>c.</unit>
<item>maraschino cherries</item>
<preparation>drained</preparation>
</ingredient>
<ingredient>
<quantity>1</quantity>
<unit>tub (8 oz.)</unit>
<item>Cool Whip</item>
<preparation>thawed</preparation>
</ingredient>
</ingredients>
<directions>
<step>Drain the oranges, pineapple, and cherries.</step>
<step>In a large bowl, combine fruit, marshmallows, and coconut.</step>
<step>Fold in the Cool Whip.</step>
<step>Chill for at least 1 hour before serving.</step>
</directions>
</recipe>
```
