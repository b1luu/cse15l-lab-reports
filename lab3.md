# Lab Report 3: Researching Commands:

Command Focus: grep

Command 1: `grep -n "specific string" (directory)`

*Description:*
>`grep -n` in particular is the location via line number of where the specific string is located in that particular file specificed in your chosen directory. This allows you to locate the specific line within the file and easier to navigate to find specifics. 


**Examples: Using `grep -n`**

Example 1: 
```

[cs15lsp23od@ieng6-203]:Media:257$ grep -n "money" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Funding_cuts_force.txt
31:The agency also receives a percentage of money from the Interest
33:percentage of the interest on money in trust accounts to Legal Aid
```
Example 2: 
```
[cs15lsp23od@ieng6-203]:Media:257$ grep -n "rent" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Rental_rules.txt    
11:None of Iowa's 99 counties regulates upkeep on rental property
13:rural renters in mobile home parks, apartments and houses with few
21:55,700 mobile homes in Iowa. Most either rent the mobile homes or
26:regulate rental units. But zoning ordinances have pushed many
47:"When you have rental properties, how the tenants take care of
50:renter complaints about sewage, roads, and vacant, vermin-infested
62:mobile home and pays $280 a month to rent the lot.

```
Sources used: [ChatGPT](https://chat.openai.com/)
