# Lab Report 3: Researching Commands:

Command Focus: **`grep`**

Command 1: `grep -n "specific string" (directory)`

*Description:*
>`grep -n "specific string" (directory)` in particular is the location via line number of where the specific string is located in that particular file specificed in your chosen directory. This allows you to locate the specific line within the file and easier to navigate to find specifics. 


**Examples: Using `grep -n "specific string" (directory)`**

Example 1: `grep -n "money" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Funding_cuts_force.txt`
```

[cs15lsp23od@ieng6-203]:Media:257$ grep -n "money" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Funding_cuts_force.txt
31:The agency also receives a percentage of money from the Interest
33:percentage of the interest on money in trust accounts to Legal Aid
```
Example 2: `grep -n "rent" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Rental_rules.txt` 
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
---

Command 2: `grep -r "specific string" (directory)`

*Description:*
> `grep -r "specific string" (directory)` allows you to search for multiple directories or subdirectories in search for a specific term. The 'r' stands for recursion, and it recursively looks for a particular word and is useful for doing a wide search that pertains to multiple files specificed within a given directory.

**Examples: Using `grep -r "specific string" (directory) `**

Example 1: `grep -r "careful" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media` 

```
[cs15lsp23od@ieng6-203]:Media:261$ grep -r "careful" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Coup_Reshapes_Legal_Aid.txt:Iwasaki's careful respect for the Long Beach program and its
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/IOLTA_INTEREST_RATE.txt:assigned, carefully delineated. As a result, what might have
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Lindsays_legacy.txt:his words carefully.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Making_a_case.txt:careful planning.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Using_Tech_Tools.txt:a hotline list, and so on," she says. She carefully notes the

```

Example 2: `grep -r "thank" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media` 

```
[cs15lsp23od@ieng6-203]:Media:262$ grep -r "thank" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Assuring_Underprivileged.txt:with which she thanks them for their time.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Bridging_legal_aid_gap.txt:all Californians. In 1999, thanks to Gov. Gray Davis and leaders in
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Commercial_Appeal.txt:growth and survival, thanks to a new focus by the Community
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Firm_to_the_Poor_Needs_Help.txt:Services are expanding, however, thanks to a $1 million public
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Philly_Lawyers.txt:Gordon thanked Task Force Co-Chairs Aretha Delight Davis and
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Pro-bono_road_show.txt:Now, thanks to a new community courthouse that opened this week
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/families_saved.txt:homes. We are also thankful for the help of the Housing Authority,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/less_legal_aid.txt:Illinois' poor will have less access to free lawyers thanks to a
```

Sources used: [ChatGPT](https://chat.openai.com/)
---

Command 3: `grep -E "specific text|other specific text" (directory)` 


*Description:*
>  `grep -E "specific text|other specific text" (directory)` where -E means to *extend* a particular search term or regular expression. The **"|"** symbol is a specifcal character notation that means "or" in regular terms. This is useful for allowing us to complete searches at once and generates efficiency. 


**Examples: Using `grep -E "specific text|other specific text" (directory)`**


Example 1: `grep -E "legal|aid" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_Society.txt `

```
[cs15lsp23od@ieng6-203]:Media:265$ grep -E "legal|aid" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_Society.txt 
LASNNY is one of the oldest and most cost-effective legal
Capital Region. LASNNY provides only needed civil legal aid --
Funding for legal aid preserves community resources and saves
out of five low-income people requiring legal help in our community

```

