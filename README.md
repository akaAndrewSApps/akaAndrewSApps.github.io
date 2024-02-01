This project was made for the primary purpose of finding all achievements that can be completed for Marvel United by the players' setup. A user can input all relevant information and the app will give a list of every achievement that can be completed in that game.

This project has the secondary purpose of allowing a user to save completed achievements so that they will no longer show up as a qualifying achievement.

This project was designed for function and does not prevent the user from selecting options that may not make sense or are not possible. This is to allow users who may be playing the game in a way not intended to still utilze this app. Users may disagree that thier setup qualifies for certain achievements for a number of reasons including thematic or errors on my part. It is up to the user to make the ultimate descision of whether or not they have accomplished an achievement.

There are four dropdowns for selecting heroes. For games with less than four characters, which dropdowns that are used does not matter. The heroes are organized by season released (with Spider-geddon being its own group) and then listed alphabetically.

There is a single dropdown for selecting a villain, with any villains that are part of a group being a single option. The villains are organized by season released (with Spider-geddon being its own group) and then listed alphabetically. The 'Infinity Campaign' checkbox is to be used if the villain selected is being used for an Infinity Battle prior to facing Thanos.

There are three Show/Hide buttons for Challeneges, Game Modes and Additional Factors. The Challenges options list all available Challenges that can be used in a game. The Game Modes options allow you to select a single Game Mode being used, with some options not implemented at this time. These options are labeled '(COMING SOON)'. The Additional Factors only contains a single option. This is because a single achievement is based on the use of a specific locaiton. Since it is the only location that is specifcally required for an achievement there was no purpose for incliding all other locations. If other future achievements require specific information that does not belong in another category, this section will gaing more options.

The selection for the Difficulty used in the game is a seperate option since only one of these can be selected. Any Difficulty other than 'Normal' will add to the Challeneges selected as the game considers these Challenges.

The Save Completed Achievements button will save all achievements that have had their checkbox checked. These achievements will no longer appear as options, even if the setup being used would qualify for that achievement.

The Clear Completed Achievements buttons will clear the user's localStorage used by the app. It is not currently implemented.

The Show All Achievements button will list every single achievement regardless of the options selected. This will also list achievements that have already been completed and saved. The Show All Remainging Achievments button will do the same, with the exception of not showing any completed and saved achievements.

app.js contains 29 functions: 
- populateDropdown1() function that populates the first hero dropdown
- populateDropdown2() function that populates the second hero dropdown
- populateDropdown3() function that populates the third hero dropdown
- populateDropdown4() function that populates the fourth hero dropdown
- populateDropdownVillains() function that populates the villain dropdown
- expand() function that adds the 'collaps' class to fieldsets based on button pressed
- getRelevantAchievements() function that takes user inputs and passes them to relevant functions
- getSelectedChallenges() function that gets the selected challenges
- getSelectedGameMode() functon that gets the select game mode
- getAdditionalFactors() function that gets any selected additional factors
- displayAchievements() function that displays all relevant achievements
- removeCompletedAchievements() function that removes any saved achievements
- getAchievements() function that gets relevant Seaosn 1 achievements
- getXAchievements() function that gets relevant Seaosn 2 achievements
- getNewAchievements() function that gets relevant new achievements
- getSpiderAchievements() function that gets relevant Spider-geddon achievements
- getVillainFights() function that gets relevant Seaosn 1 Villain Fights achievements
- getXVillainFights() function that gets relevant Seaosn 2 Villain Fights achievements
- getSpiderVillainFights() function that gets relevant Spider-geddon Villain Fights achievements
- getHeroFeats() function that gets relevant Seaosn 1 Hero Feats achievements
- getXHeroFeats() function that gets relevant Seaosn 2 Hero Feats achievements
- getSpiderHeroFeats() function that gets relevant Spider-geddon Hero Feats achievements
- checkAntiHero() function that checks selected heroes for anti heroes
- checkStartingHandHeroes() function that checks selected heroes for heroes with Starting Hand cards
- getAvailableTeams() function that checks selected heroes for available teams
- saveCompletedAchievements() function that saves all checked achievements as completed
- clearCompletedAchievements() function that clears all saved achievements
- showAllAchievements() function that shows all achievments
- showRemainingAchievements() function that shows all non-completed achievments
