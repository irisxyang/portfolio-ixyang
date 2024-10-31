---
layout: doc
---

<script setup>
  import { withBase } from 'vitepress';
</script>

# User Study 2 (Unedited): John

## Task 1: Basic Registration

- No trouble navigating to registration page, clear heading on navbar
- A little bit of confusion on the user weighting, but understood after reading description
- No issues logging out after navigating to Settings

## Task 2: Restaurant Exploration

- Easy to find Restaurant Search page from the Home page
- Did not expect search to be case-sensitive, could have been hard to match correct capitalization
- Thought the Restaurant page was pretty clearly formatted
- Weightings were displaying "NaN" at first, but once refreshed page it worked as expected
- Could be nice to have a visual of the weighting scale to really give a sense of what is considered "good" vs "bad"
- The numbered weighted average was good once you understood the scale, but would have been nice to have a reminder (a rating of 1 seems bad but is actually a bit above average)
- Could be nice to sort or filter reviews based on score, or even filter restaurants based on weighted average

## Task 3: Reviewing

- Would be nice to have a dedicated Add Review button in the navbar
- Adding review from a certain restaurant made sense, but what if they wanted to just create a review before searching for a restaurant
- Review interface appeared easy to use and pleasing to the eye
- Made sense that after reviewing, automatically navigated back to the Home page (with recent review at top)

## Task 4: I Didn't Like That Review... (Review Deletion)

- Nice that all reviews written by session user had a clear "Edit Review" button on all views of the review, not like he had to navigate back to own profile
- Editing review interface was pretty easy to use, but didn't like that the scores were reset to zero instead of displaying previously inputted scores
- Was able to update review, made sense that it navigated to the profile page afterwards
- Delete works as expected

## Task 5: New Priorities (User Weighting Editing)

- Was easily accessible to navigate to "Settings"
- Would have also been okay if the "Settings" button was on the Profile page
- Settings update went well, made sense that you might want to readjust weightings

## Debrief: Thoughts and Impressions

**What worked well?**

- The interface was very pleasant, especially liked the color scheme
- The weighted averaging generally worked well (with a few refresh kinks when initialized)
- Generally the site was easy to use, with a couple of kinks but most of the functionality worked as expected

_What is an example of something that worked as expected?_

- Most of the navigation and routing was pretty intuitive, except maybe the logout
- Could maybe also add more routing capabilities between pages

**What do you think could be improved on?**

- Maybe adding some restrictions for password options for security measures (such as needing to add special characters but not letting you use passwords that are too short)
- Making search not case-sensitive could make the search much easier for users since they don't need to match the name of the restaurant exactly
- Adding a visual for reference to display the weighted averages on each restaurant could be a great way of emphasizing the actual scale of the averages

_Why was this unintuitive for you?_

- Made sense once you got the hang of the averaging scale (zero as average), but initially was seeing all the ratings as extremely low
- 1 on the scale is above average, but intuitively seems like a very bad score in context of a typical 5-star rating
