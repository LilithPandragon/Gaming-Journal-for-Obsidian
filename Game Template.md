<%*
const title = await tp.system.prompt("Game Title");
if (title) { await tp.file.rename(title); }
const platforms = ["PC", "Steam Deck", "PS5", "PS4", "PS2", "Switch", "Switch2", "Gameboy", "GameboyColor", "GameboyAdvanced", "Sega Dreamcast", "Other"];
const platform = await tp.system.suggester(platforms, platforms, false, "Played on?");
const year = await tp.system.prompt("Release Year");
-%>
---
cssclasses:
  - gamejournal
release_year: <% year %>
played_on: <% platform %>
started_on: <% tp.date.now("YYYY-MM-DD") %>
finished_on: 
completed: false
dropped: false
rating: 0
tags:
  - game
---

> [!game] Why I wanted to play this
> 
> 
> 

> [!scene] That one scene that thrilled / annoyed me
> 
> 
> 

> [!liked] What I liked about it
> 
> 
> 
> 

> [!sentence] In one sentence
> | | |
> |---|---|
> | **Graphics** | |
> | **Sound** | |
> | **Story** | |
> | **Gameplay** | |
> | **Controls** | |
> | **Difficulty** | |

> [!rating] My Rating
> - [ ] 
> - [ ] 
> - [ ] 
> - [ ] 
> - [ ] 
> - [ ] 
> - [ ] 
> - [ ] 
> - [ ] 
> - [ ] 
