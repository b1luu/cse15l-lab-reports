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


Command 2: `grep -r "specific string" (directory)`

*Description:*
> `grep -r` allows you to search for multiple directories or subdirectories in search for a specific term. The 'r' stands for recursion, and it recursively looks for a particular word and is useful for doing a wide search that pertains to multiple files specificed within a given directory.

**Examples: Using `grep -r `**

Example 1:

```
[cs15lsp23od@ieng6-203]:Media:259$ grep -r "about" /home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media                    
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/5_Legal_Groups.txt:agencies about $375,000 each year. My assistant, Charity
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/AP_LawSchoolDebts.txt:In the law study, about 68 percent of public interest employers
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/AP_LawSchoolDebts.txt:about $35,000, while government pays $40,000 to $45,000.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/A_helping_hand.txt:She was about to run out of means to pay back those loans when
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/A_helping_hand.txt:represent poor clients against wealthy landlords, a calling about
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/A_helping_hand.txt:others in a community that cares about access to justice for the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/A_helping_hand.txt:Mintie also started to ask questions about the medical field.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Anthem_Payout.txt:recent mailing by Anthem, the Indianapolis-based insurer, of about
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Anthem_Payout.txt:about $22,000 went to people who had been with Anthem the longest,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Anthem_Payout.txt:Christmas, many aid recipients were confused about why they got the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Assuring_Underprivileged.txt:or through the reports from their advocates, about how alien a
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Assuring_Underprivileged.txt:While unprepared lawyers annoy her, several things about the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Assuring_Underprivileged.txt:about pro bono, [and] getting law firms more involved in a [formal]
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Attorney_gives_his_time.txt:"Even then, he would worry about pro bono work and has done it most
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Avoids_Budget_Cut.txt:decisions about who to turn away.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Barnes_pro_bono.txt:his surprise loss to Sonny Perdue on Nov. 5. Asked about his legacy
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Barnes_pro_bono.txt:not cash in, and do something he really does care about," said
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Barr_sharpening_ax.txt:questions about the Legal Services Corp.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Barr_sharpening_ax.txt:The Legal Services Corp. came about in 1974 under President
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Barr_sharpening_ax.txt:spelling out his questions about the organization.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/BergenCountyRecord.txt:County's federal funding - about $385,000 this year - to Northeast
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/BergenCountyRecord.txt:about $1.6 million could follow, although Thorne noted the state
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/BergenCountyRecord.txt:"This is not about job security for me and Maxim," Atlas said.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/BergenCountyRecord.txt:Passaic County Legal Aid works on behalf of about 4,000
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/BergenCountyRecord.txt:individuals each year, and provides lowfee legal help for about 20
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Bias_on_the_Job.txt:study, which extrapolated from federal data on about 200,000 large
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Bias_on_the_Job.txt:and midsize employers, concludes that about two million workers
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Boone_legal_service.txt:Schroeder has upheld the outfit alone, taking on about 60 clients a
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/City_Council_Budget.txt:current finding of about one-third.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Civil_Matters.txt:pro bono work by private attorneys. That's about $170 million a
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/CommercialAppealMemphis2.txt:Several law firms have donated about $25,000 and the Community
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/CommercialAppealMemphis2.txt:talking to a lawyer about her pending eviction from a high-rise
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Commercial_Appeal.txt:The nonprofit law firm has about 40 employees and an annual
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Coup_Reshapes_Legal_Aid.txt:"We had a discussion about what our separate views were,"
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Coup_Reshapes_Legal_Aid.txt:about us and deliver services to them," Dudovitz said. "We have
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Coup_Reshapes_Legal_Aid.txt:about the changeover," Wheeler said.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Coup_Reshapes_Legal_Aid.txt:effective if [we are] thoughtful about how we employ staff and the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Coup_Reshapes_Legal_Aid.txt:community for their ideal marriage, Dudovitz had no regrets about
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Court_Keeps_Judge_From.txt:The funds are part of about $2.75 million in interest that
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Court_Keeps_Judge_From.txt:until all legal questions about his authority were resolved.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Disaster_center.txt:materials about various assistance programs. Among the disaster
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Do-it-yourself_divorce.txt:starts at about $1,500. Others just want to be in control of the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Do-it-yourself_divorce.txt:Vermont, said he worries most about people who have reading
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Domestic_Violence_Ruling.txt:group. "But we're talking about people in long-term relationships.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Domestic_violence_aid.txt:For details about the Domestic Violence Legal Assistance
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Donald_Hilliker.txt:foundation has an annual budget of about $12 million. Of that,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Donald_Hilliker.txt:about $6.4 million has in the past come from the Legal Services
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Eviction_law.txt:The commission administers about 3,500 public housing units in
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Eviction_law.txt:evicted from public housing about a year ago with several young
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Eviction_law.txt:"She didn't know about it," Curry said of the drug deal.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Farm_workers.txt:The lettuce workers, talking about their incident last week,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Farm_workers.txt:Recent research raises questions about the connection between
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Firm_to_the_Poor_Needs_Help.txt:provided about a third of the donations. Businesses and
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Firm_to_the_Poor_Needs_Help.txt:attorney about civil legal problems, including rent and contract
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Firm_to_the_Poor_Needs_Help.txt:talk about our legal system. That phrase is etched on our U.S.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/FortWorthStarTelegram.txt:about $1.03 million. The legal aid group cleared about 8,300 cases
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/FortWorthStarTelegram.txt:staff of about 100 employees, including attorneys and support
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/FortWorthStarTelegram.txt:has distributed about $8 million statewide. Besides the IOLTA
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/FortWorthStarTelegram.txt:about $555,000.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/FortWorthStarTelegram.txt:On Dec. 9, the U.S. Supreme Court will hear arguments about the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Free_Legal_Assistance.txt:of Social Ecology, said users were overwhelmingly positive about
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Free_Legal_Assistance.txt:about $800 if he had relied on a lawyer, he said. "It was a lot
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Free_legal_service.txt:Legal office by about $50,000," Wilson said Thursday. "That means
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Free_legal_service.txt:about $920,000 in congressional funding annually.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Free_legal_service.txt:about 35,000 fewer people who are eligible for LSC services.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Free_legal_service.txt:The Illinois General Assembly has appropriated about $500,000
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Funding_cuts_force.txt:about 24,000 low-income people annually. Legal Aid lawyers help
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Funds_Shortage.txt:about their problems.... It's usually the leadership," she
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Funds_Shortage.txt:Fund, which distributes the interest income, there are about 250
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Ginny_Kilgore.txt:about events occurring in our country during those times in the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Greedy_Generous.txt:even say about our profession? Do most of us identify with one or
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Greedy_Generous.txt:large law firms to vent and share information about salaries,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Greedy_Generous.txt:information about the latest salary increase or layoffs is shared
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Greedy_Generous.txt:and more about world affairs, political opinions and advice to
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Greedy_Generous.txt:The site sets forth information about the Legal Aid Society and the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Greedy_Generous.txt:same firms that are talking about firing people are pretty much the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Greedy_Generous.txt:see so much discussion about some very non-greedy subjects such as
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Greedy_Generous.txt:about money. It seems that young lawyers only want to work for
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Greedy_Generous.txt:up a $100k in student loans that require about $1000 a month or
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Greedy_Generous.txt:more payments and you too will care about money."
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Greedy_Generous.txt:generous than just about any other profession. A report
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/GreensburgDailyNews.txt:found time to help out in causes he feels strongly about. It was
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/GreensburgDailyNews.txt:speak nationally about our system," Shepard said. "That is a great
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Hard_to_Get.txt:What about the less theatrical, but equally troubling, civil
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Hard_to_Get.txt:full- time staff of about 75 lawyers, paralegals, intake
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Helping_Out.txt:"basis" or "stepped-up basis" to be about as easy to follow as the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Higher_court.txt:those of surrounding states and would raise about $1.3 million a
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/It_Pays_to_Know.txt:agents of Utah Nonprofit Housing to find out about her
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Justice_for_all.txt:a staff of 500, including about 200 attorneys.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Justice_for_all.txt:more than just a job. This is about changing people's lives."
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Justice_for_all.txt:depends on human beings caring about other human beings."
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Kiosks_for_court_forms.txt:County with about $800,000 in grants. The program avoids legal
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Law-school_grads.txt:In 2001, median private law school tuition was about $23,000 a
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Law-school_grads.txt:'A lot of people I went to law school with were fired up about
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Law-school_grads.txt:tuition climbed from about $15,000 to $23,994 during the past 10
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Law-school_grads.txt:student body of about 1,000, and CU's population is about half
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Law_Award_from_College.txt:passionate about their concerns. She's good at looking at the big
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Law_Schools.txt:"We're talking about training real community lawyers," said Stua
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Law_Schools.txt:about malpractice insurance? Such are the sobering questions,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Lawyer_Web_Survey.txt:employment, we have no idea about who continues in the field, who
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal-aid_chief.txt:But after about a quarter century in private practice, he
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal-aid_chief.txt:Right now, Nebraska Legal Services, which handles about 95
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal-aid_chief.txt:services. That's about 8,500 cases a year.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal-aid_chief.txt:that Nebraska's low-income residents will be involved in about
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_Society.txt:Our elected officials, and all who are concerned about providing
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_attorney.txt:"I've been reading a lot about Buddhism," she added. "I just
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_campaign.txt:poor persons in West Virginia. This compares to about one attorney
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_in_Clay_County.txt:"Study after study shows unmet needs to be about 80 percent," he
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_in_Clay_County.txt:The ability to handle more cases is about to take a big jump,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_in_Clay_County.txt:"Currently, we spend about $250,000 a year in Clay County, which
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_in_Clay_County.txt:is about 8 percent of our budget," said Figgins, adding that Clay
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_in_Clay_County.txt:County clients also represent about 8 percent of the total "poverty
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_in_Clay_County.txt:about $60,000 a year, of which approximately $40,000 will be spent
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_in_Clay_County.txt:about 75 percent of the women who come to her agency in search of
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_looks_to_legislators.txt:proposed legislation is expected to generate about $1.5
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_Aid_looks_to_legislators.txt:Because of about $300,000 in cuts, Kentucky Legal Aid in Bowling
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_hotline.txt:officials about the way the hotline's grant application had been
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_hotline.txt:other cuts in staff hours. Last year, about 7,200 people were given
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_services_for_poor.txt:Statewide, Legal Aid will lose about $800,000 in federal funds -
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_services_for_poor.txt:a cut of about 13 percent from the $6 million it got this year from
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_services_for_poor.txt:The state also is facing the loss of about $460,000 - nearly all
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_services_for_poor.txt:facing a decline of about $100,000 in funds from interest collected
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_services_for_poor.txt:about $260,000 out of a budget of about $2.2 million. All of the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_services_for_poor.txt:Bricking said he expects to lose about $170,000 out of an annual
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_services_for_poor.txt:budget of about $3 million.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_services_for_poor.txt:Unless Congress increases funding, Kentucky will lose about
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_services_for_poor.txt:poverty rate declined about 3 percent under the latest Census
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_services_for_poor.txt:Legal Aid officials are particularly worried about impoverished
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_system_fails_poor.txt:enough or think nothing can be done about the problem.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_system_fails_poor.txt:ugh few of those surveyed were able to get legal help, about 71
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_system_fails_poor.txt:Attorneys working for Legal Services help about 50,000 people a
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_system_fails_poor.txt:released in 1994 which found about 20 percent of the nation's poor
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_system_fails_poor.txt:about $20 a person can get a cup of coffee and a consultation with
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_system_fails_poor.txt:just there to give them some initial direction about whether they
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Legal_system_fails_poor.txt:officials are concerned about the findings, their assistance can
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Library_Lawyers.txt:"I knew about the Vallejo program and wanted to see if it would
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Library_Lawyers.txt:not have to worry about seeing a biased attorney."
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Library_Lawyers.txt:attorneys per night right now, we can only see about 15 people each
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Lindsays_legacy.txt:member, invited her to lunch to talk about "some ideas he had for
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Lindsays_legacy.txt:about their cases," Broker says. "He had such a depth of
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Major_Changes.txt:fails. Bronx Legal Services raises about $450,000 a year through
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Making_a_case.txt:The attorney can give basic advice about what will need to be
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Making_a_case.txt:anything filed with a court, nothing can be done about your request
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Marylands_Legal_Aid.txt:where federal subsidies are about to run out.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Marylands_Legal_Aid.txt:only about 20 percent of eligible potential clients are served Co
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/NJ_Legal_Services.txt:first step in a process that will also cost them about $1.5 million
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/New_Online_Resources.txt:those agencies can update the online information about the services
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/New_Online_Resources.txt:area contains information for attorneys to learn about that area of
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/New_funding_sources.txt:site lists about 600 titles from the past 20 years, with reviews of
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/New_funding_sources.txt:about one-third of the books.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Nonprofit_Buys.txt:program. The two programs are currently housed in buildings about a
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Nonprofit_Buys.txt:The organization raised about $60,000 to purchase the A Street
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Nonprofit_Buys.txt:For information about reprinting this article, go to
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Oregon_Poor.txt:She asked to see the title, wondering about previous owners and the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Owning_a_Piece.txt:ground in Harlem Built of brick and the width of about four
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Owning_a_Piece.txt:Legal Aid has about 25 staff members in its Harlem office,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Paralegal_Honored.txt:that meet on a volunteer basis to learn about new programs and
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Politician_Practices.txt:Chapel Hill -- There must be something different about former
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Politician_Practices.txt:Georgia governors. I was never crazy about Jimmy Carter while he
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Politician_Practices.txt:tried to do something about the Confederate symbol on the Georgia
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Politician_Practices.txt:money he has." But study after study shows that about 80 percent of
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Politician_Practices.txt:But that's about as far as the sentiment goes.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Politician_Practices.txt:I love Jimmy Carter. I'm starting to feel the same way about Roy
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Poverty_Lawyers.txt:"There are reasons why people do this work, it's about larger
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Poverty_Lawyers.txt:intellectual issues about the role of government in people's lives,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Poverty_Lawyers.txt:lawyers do not worry about what they owe.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Poverty_Lawyers.txt:"But public service wasn't something I thought about," he said.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Pro-bono_road_show.txt:The organization deals with about 10,000 poor clients a year who
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Pro-bono_road_show.txt:need legal help, and Hall estimates about 260,000 people in Bexar
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Pro-bono_road_show.txt:want to talk about the case anymore.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Pro_Bono_Services.txt:The Chicago Bar Foundation, which supports about 40 legal-aid
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Pro_Bono_Services.txt:But the legal-aid groups don't know how to spread the word about
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Pro_Bono_Services.txt:even think about [public relations] and marketing because all of
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Pro_Bono_Services.txt:for the Center for Conflict Resolution about a year ago. Her
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Program_Lodges.txt:just about everywhere as shoppers hit stores for their annual
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Program_Lodges.txt:he joined about six other lawyers doing pro bono work.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Raising_the_Bar.txt:feeling pleased about the award.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Raising_the_Bar.txt:per lawyer to make up for the shortfall. Just about everyone came
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Raising_the_Bar.txt:Lalley also is enthused about other bar efforts on behalf of the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Rental_rules.txt:renter complaints about sewage, roads, and vacant, vermin-infested
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Retirement_Has_Its_Appeal.txt:"This is an effort to do something about that, while giving
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/RoanokeTimes.txt:Asked later about the program's future, Harley said it is only
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Rumble_in_the_Bronx.txt:legislature cut LSC funds by 31 percent, to about $280 million.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Rumble_in_the_Bronx.txt:million budget, about 40 percent of which comes directly from LSNY,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Service_Agency.txt:helped about 250,000 people over those years with urgent legal
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Service_Agency.txt:sources, general unrestricted funds. Now that is about half. The
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Service_Agency.txt:The annual operating budget is about $3.4 million, Heald said.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/State_funding.txt:one administrator, Mathews said. The agency has only about a half
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Survey.txt:For those worried about the indebtedness of young attorneys --
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Survey.txt:afford to think about taking low-paying jobs.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Survey.txt:at about $40,000. Staff attorney positions at city and federal
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Survey.txt:specific about what kinds of debt burdens students are going to
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Survey.txt:concerned about his graduates' debt burdens. He tells students: "If
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Survey.txt:Harbaugh expressed skepticism about the cent ral thesis of "Paper
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Survey.txt:got back from a job fair in Washington where I identified about two
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Targeting_Domestic_Violence.txt:Said Palazzolo, "One of the things that excites me about it is
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Terrorist_Attack.txt:about 36 hours per year, which is down significantly from an
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Texas_Lawyer.txt:"What you normally think of a hotline doing is spending about 15
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Texas_Lawyer.txt:about five years ago -- has made "a tremendous difference in our
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Texas_Lawyer.txt:Antonio Center opened about 5,000 client files stemming from calls
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Texas_Lawyer.txt:domestic violence who are given information about shelters where
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Texas_Lawyer.txt:Hall says that about 20 UT law students will be needed to answer
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Texas_Lawyer.txt:careers about the need for pro bono service.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/The_Bend_Bulletin.txt:Office of Legal Aid Services Wednesday evening about 30 minutes
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/The_Bend_Bulletin.txt:A little car trouble wasn't about to keep him from delivering
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/The_Bend_Bulletin.txt:closing courthouse doors on anybody," Balmer told about 20 lawyers,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/The_Bend_Bulletin.txt:but only about 111 lawyers (less than 1 percent of the bar) compose
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/The_Bend_Bulletin.txt:Federal funding accounts for about one third of Oregon's
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/The_Columbian.txt:The interest from the pooled money adds up to about $6 million
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/The_Columbian.txt:"We only can help right now about one out of five people who ask
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/The_State_of_Pro_Bono.txt:But what about the months before Sept. 11? From all the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/The_State_of_Pro_Bono.txt:translate into about 1,300 hours a year, more than half a
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Too_Crucial_to_Take_Cut.txt:responsibility to serve the civil legal needs of about 550,000 poor
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Too_Crucial_to_Take_Cut.txt:those who need our help. It is unfathomable to think about the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Towson_Attorney.txt:people something else to think about the next time they hear a
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Towson_Attorney.txt:Wagonheim said he initially hoped to recruit about 300
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Towson_Attorney.txt:After contacting attorneys about Take 2, Wagonheim is beginning
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Towson_Attorney.txt:matters, said that Take 2 "is not charity. It's about the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Unusual_Woodburn.txt:about pesticides in the fields.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Unusual_Woodburn.txt:Willamette Valley to talk with workers about their legal rights.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Using_Tech_Tools.txt:uncertainty about legal fees and their fear of the profession.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Using_Tech_Tools.txt:about divorce; MyCounsel.com is aimed at small businesses, and
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Using_Tech_Tools.txt:are devoid of explanations about what public interest lawyers
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Valley_Needing_Legal_Services.txt:takes on about 10,000 cases per year with a staff of eight or nine
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Valley_Needing_Legal_Services.txt:Corp. this year, the Valley receives about $15 million to $20
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Valley_Needing_Legal_Services.txt:million and employs about 37 staff lawyers. Organizations that
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Weak_economy.txt:weighs what to do about an expected $1.2 billion state budget
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Weak_economy.txt:year into Maryland legal services and about $160 million into such
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Weak_economy.txt:those who want to leave their husbands but are unsure about their
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Weak_economy.txt:judgment. She is about to return to court for a hearing to clear
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Weak_economy.txt:every new legislator an orientation package about legal help for
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Wilmington_lawyer.txt:"The award says a lot about the legal profession, that it places
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Wilmington_lawyer.txt:also says a lot about the Delaware Bar, which nominated her.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Workers_aid_center.txt:in North Hills for two years and serves about 100 people each
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Workers_aid_center.txt:when I asked my boss about the overtime, he told me I could walk
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Working_for_Free.txt:with poverty was reading newspaper articles about unscrupulous
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Working_for_Free.txt:Zucker said. "They seemed to be more passionate about their weekend
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Working_for_Free.txt:disputes. Through the center, about 30 indigent clients a year
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/Working_for_Free.txt:Spanish about divorce proceedings to a dozen people seated around a
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/balance_scales_of_justice.txt:financial help -- about $6,000 a year -- to provide speech therapy
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/balance_scales_of_justice.txt:services for only about one in every five people who ask for them,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/balance_scales_of_justice.txt:Legal Aid spends about $2 million a year culled from a variety
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/balance_scales_of_justice.txt:services. The office serves about 4,500 people a year. About 81
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/defend_yourself.txt:are so rare that statistics about the practice generally are not
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/defend_yourself.txt:wealthier litigants. However, about 20 percent of self-represented
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/defend_yourself.txt:about pro-se litigation.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/families_saved.txt:"We cannot say enough about how relieved we are that this is
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/fight_domestic_abuse.txt:cases next year. The group closes about 2,500 cases a year.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/fight_domestic_abuse.txt:lost about $120,000 in grant money due to a decrease in the poverty
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/grants_fail_to_come.txt:having to worry about getting paid.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/grants_fail_to_come.txt:years, leaving about a year ago over a dispute with management in
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/grants_fail_to_come.txt:about Smith from the friend of a friend two months ago.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/grants_fail_to_come.txt:The man"s experience had left him bitter about the legal system,
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/help_rent-to-own_tenants.txt:Bryant said he read about the issue in a July News & Advance
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/help_rent-to-own_tenants.txt:director) Ed McCann about it," Bryant said Monday. "I asked them to
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/help_rent-to-own_tenants.txt:"I was a little concerned about it and wanted to see if there
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/help_rent-to-own_tenants.txt:June 27, 2001 article about rent-to-own contracts.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/highlight_Senior_Day.txt:"But it's like trying to tell a stranger about rock 'n'
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/highlight_Senior_Day.txt:about how they have improved the lives of older Oklahomans.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/less_legal_aid.txt:in Illinois will lose about $920,000 in congressional funding
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/less_legal_aid.txt:about 35,000 fewer people who are eligible for LSC services because
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/less_legal_aid.txt:of low income, about $22,000 a year for a family of four, Kleiman
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/less_legal_aid.txt:The Illinois General Assembly has appropriated about $500,000
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/man_on_national_team.txt:years. It's a friendship that began spontaneously about five years
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/man_on_national_team.txt:president. And while he's nervous about his new duties, it's the
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/man_on_national_team.txt:At about the same time, El Paso gallery owner Adair Margo was
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/man_on_national_team.txt:told me all about you,' " he said.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/man_on_national_team.txt:about them, which is why the Bushes have always wanted to see them
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/predatory_loans.txt:what to do about such loans.
/home/linux/ieng6/cs15lsp23/cs15lsp23od/stringsearch-data/technical/government/Media/stringsearch:pro bono work by private attorneys. That's about $170 million a
```


