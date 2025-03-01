---
title: playercreateinfo_items
type: worlddb
category: P
layout: single_markdown
---

# playercreateinfo_items
This table contains the custom applied items for new created players.

## Structure

Field               | Type          | Default | Comment
------------------- | ------------- | ------- | -------
[build](#build)     | smallint(6)   | 12340   | key
[race](#race)     | smallint(6)   | 0   | key
[class](#class)     | smallint(6)   | 0   | key
[protoid](#protoid) | mediumint(10) | 0       |        
[slotid](#slotid)   | tinyint(3)    | 0       |        
[amount](#amount)   | tinymint(3)   | 0       |        

### build

Build number used by AE to determine if the data is for our current compiled version.

### race

...

### class

...

### protoid

The item entry ID from [item_properties](/Wiki/database/world/item_properties/ "Item properties") table.

### slotid

The slot ID of the character:

<pre>
0 = head
1 = neck
2 = shoulder
3 = shirt
4 = chest
5 = waist
6 = legs
7 = feet
8 = wrists
9 = gloves
10 = finger1
11 = finger2
12 = trinket1
13 = trinket2
14 = back
15 = main hand
16 = off hand
17 = ranged
18 = tabard
</pre>

<pre>
19 - 22 = inventory bag slots (the 4 bagslots without the main backpack)
23 - 39 = inventory backpack slot (main backpack)
67 - 73 = bankslots
86 - 118 = keyring
</pre>

### amount

ATTENTION: You can't use a value > "1" on the playerslots ( You cant stack two shoulders on you :-) )
{: .info }