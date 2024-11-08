---
title: Assignment 5 - Notes
layout: doc
---

## Concepts Plan

home screen:
restaurant search
profile page
my groups page
reviews feed (of friends) -- review component
"search a restaurant to write a review"

restaurant results
restaurant component

restaurant page
write a review!

my groups page
create new group
view group

group page
restaurant component

user page
user review components
user groups

## Vue.js

index.html:

- main entry point
- divs, etc.
- in main.ts, we create the Vue app

instead of having html, css, js, we have:

- script block for all of js fns
- html template block for html
- style block for css
  all in the SAME PAGE

reactive variable

- "ref" from vue
- should never mess with reactive variable direction (ex reassign, etc.)
- to make change to ref, we do ref.value!!
  in script:
  const msg = ref("this ref holds this message");

in template:
{{ msg }}
<input type="text" v-model="message"/>

- binds the input to the "message" ref
  v-model="message": 2 way data bind

1. v-bind:value="message": update input field when message ref is changed by something else
2. v-on:input="event => message = event.target.value": updating input text changes the message ref. listening to changes in input--every time there is a change to the input text (new inp event), we update message variable to value of input

create COMPUTED property (not reactive variable)

- takes FUNCTION input in init
- deriving new value from some other value
- make sure to grab .value with any ref variable in the js block
  const msg = computed(() => { return message.value.split('').reverse().join(''); });
- will update computed property if there is a REF in computed that changes
- if no ref, then will not update automatically

- a regular function will constantly update/refresh with any change to interface
  (i.e. will call the function again each time to refresh bc it doesnt know any better)
