learn reveal js

- intro to revel.js
    - http://lab.hakim.se/reveal-js/#/
- and it's source (study this template)
    - https://github.com/hakimel/reveal.js/blob/master/index.html

# Make your own presentation


create git repo for presentations

    mkdir presentations
    cd presentations
    git init

make reveal.js as submodule

    git submodule add https://github.com/hakimel/reveal.js revealjs

add index.html (or some other presentation-name-for-some-crap.html)

Your html has to have this structure:

- html
    - head (front matter)
        - title
        - meta
        - link css
        - script
    - body (has 2 sections)
        - div reveal (all slides are here)
            - div slides (each section is a slide)
                - section (first one)
                - section
                - section
        - script (more than one)
        - script
        - script

## Authoring with markdown

Given I use Rubymine I need to fix the automatic reformatter so it does not mess up my `pre.code` sections and my `<section data-markdown>`

Rubymine Settings > Code Style > HTML section

- tab: Tabs and Indents
    - numbers 2, 4, 8
- tab: Other
    - Insert new line before:
        -  add `section` entrey
    - Do not indent children of:
        - add `code` and `section data-markdown`
    - Keep whitespaces inside:
        - add `code`, `section`, `section data-markdown`


## Running

change theme at runtime

index.html?theme=night
reloads `index.html?theme=night#/` in the theme night you specify

Themes from dark to light are: night, moon, default, sky, beige, serif, solarized, simple


