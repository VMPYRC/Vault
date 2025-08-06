---
created: 2025-07-22
modified: 2025-07-27
description:
aliases:
tags:
    - Project
---

# Notes

## Surnames

- https://www.gramps-project.org/wiki/index.php/Names_in_Gramps#Origin_Attributes
- UNKNOWN: indeterminate origin
- CUSTOM: Custom user defined origin
- NONE: no given origin
- GIVEN: name was bestowed on the individual (includes 'John Doe' names)
- PATRILINEAL: name was inherited from father's family name
- MATRILINEAL: name was inherited from mother's family name
- PATRONYMIC: name is derived from father's given name
- MATRONYMIC: name is derived from mother's given name
- FEUDAL: name refers to the holding of land in a fief
- PSEUDONYM: name is fictitious
- OCCUPATION: name refers to the trade employing the person
- ==INHERITED: name was based on the parent name(s)==
- ==TAKEN: name was chosen by the individual, including when adopting a spouse's surname==

## Event Types

- https://gramps-project.org/wiki/index.php/Events_in_Gramps

### Built-In

- Birth
- Baptism
- Death
- Stillbirth
- Burial
- Cremation
- Adopted
- Family
    - Engagement
    - Marriage
    - Divorce
    - Annulment
    - Marriage Settlement
    - Marriage License
    - Marriage Contract
    - Marriage Banns
    - Divorce Filing
    - Alternate Marriage - Cohabitation, Common Law Marriages, Civil Unions, Domestic Partnerships
- Religious
    - Christening
    - Adult Christening
    - Confirmation
    - First Communion
    - Blessing
    - Bar Mitzvah - when a Jewish boy reaches age 13
    - Bat Mitzvah - when a Jewish girl reaches age 13, also known as "Bas Mitzvah"
    - Religion
- Vocational
    - Occupation
    - Retirement
    - Elected
    - Military Service
    - Ordination
- Academic
    - Education
    - Degree
    - Graduation
- Travel
    - Emigration - leaving one's homeland with the intent of residing elsewhere
    - Immigration - An event of entering into a new locality with the intent of residing there
    - Naturalization - obtaining citizenship
- Legal
    - Probate
    - Will
- Residence
    - Residence - the act of dwelling at an address for a period of time
    - Census
    - Property
- Other
    - Cause of Death
    - Medical Information
    - Nobility Title
    - Number of Marriages

### [Custom](https://gramps-project.org/wiki/index.php/Custom_Event_Types)

- News
- Vacation
- Award
- Gathering
- Membership - Club, Society, Organization
- Birthday
- Memory

## Relationship Types

- https://www.gramps-project.org/wiki/index.php/GEPS_001:_Relationship_type_event_link
- Built-In
    - **Married**: any religious union
        - Divorced (Add event)
    - **Civil Union**: all other civil legal union
    - **Unmarried**: a family with no bonds, or a family living together without a mutual love
    - **Unknown**: Unknown
- CUSTOM
    - Cohabitation: the state of living together and having a romantic relationship without being married
    - Dating
        - Ex-Partner
    - Engaged
        - Ex-Engaged

# Customize Gramps / Modify Files

> [!warning] Warning
> I use this software primarily for fantasy / imaginary worldbuilding, so numbers are exaggerated

## Preferences >> Name Format

Title Given (Call) "Nickname" Surname Suffix

## gramps.ini

`AppData\Roaming\gramps\gramps60\gramps.ini`

- REMOVE the ;;
    - date-about-range=100000000000
    - date-after-range=100000000000
    - date-before-range=100000000000
- max-age-prob-alive=100000000000
- max-sib-age-diff=100000000000
- 100 billion: 100,000,000,000 = 100000000000

### tool_options.xml

`AppData\Roaming\gramps\tool_options.xml`

```
<option name="MAX_AGE_PROB_ALIVE" value="100000000000"/>
<option name="MAX_SIB_AGE_DIFF" value="100000000000"/>
```

### syncAssociations.py ([Custom Associations](https://gramps-project.org/wiki/index.php/Roles,_Relationships_%26_Associations))

```
AppData\Roaming\gramps\gramps60\plugins\SyncAssociations\syncAssociations.py
```

See https://github.com/VMPYRC/Lab/blob/main/python/syncAssociations.py

## Zodiac Signs

```
♈︎ Aries ♈ 21 March - 20 April 🐏
♉︎ Taurus ♉ 21 April - 21 May 🐂
♊︎ Gemini ♊ 22 May - 21 June 🧑‍🤝‍🧑
♋︎ Cancer ♋ 22 June - 23 July 🦀
♌︎ Leo ♌ 24 July - 23 August 🦁
♍︎ Virgo ♍ 24 August - 23 September 👧
♎︎ Libra ♎ 24 September - 23 October ⚖️
♏︎ Scorpio ♏ 24 October - 22 November 🦂
♐︎ Sagittarius ♐ 23 November - 21 December 🏹
♑︎ Capricorn ♑ 22 December - 20 January 🐐
♒︎ Aquarius ♒ 21 January - 19 February 🏺
♓︎ Pisces ♓ 20 February - 20 March 🐟
```

# Resources

|      Content       | Link                                               |
| :----------------: | -------------------------------------------------- |
|        Blog        | https://gramps-project.org/blog/                   |
|       GitHub       | https://github.com/gramps-project                  |
|  GitHub Releases   | https://github.com/gramps-project/gramps/releases  |
|  Bugs, Changelog   | https://gramps-project.org/bugs/changelog_page.php |
| Discussions, Forum | https://gramps.discourse.group/                    |
|        Wiki        | https://gramps-project.org/wiki/                   |
