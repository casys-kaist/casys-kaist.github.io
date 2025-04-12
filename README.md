# AI Deadlines (KAIST CASYS Fork)

This is a fork of the original [ai-deadlines](https://github.com/abhshkdz/ai-deadlines) project, created by [Abhishek Das (abhshkdz)](https://github.com/abhshkdz).
This version is maintained by the [Computer Architecture and Systems Laboratory (CASYS) at KAIST](https://casys.kaist.ac.kr/).

Countdown timers to keep track of a bunch of CV/NLP/ML/RO/Systems conference deadlines relevant to KAIST CASYS.

## Local Development Setup

```bash
git clone https://github.com/casys-kaist/casys-kaist.github.io.git
cd casys-kaist.github.io
bundle add jekyll
bundle exec jekyll serve
```


## Contributing

Contributions are very welcome! Please submit Pull Requests to the [casys-kaist/casys-kaist.github.io](https://github.com/casys-kaist/casys-kaist.github.io/) repository.

**Adding/Updating Conferences:**
- Add or edit the relevant YAML file under the **`./_data/conferences/`** directory, e.g., **`./_data/conferences/2026.yml`**. Use the year of the conference date, not the submission deadline year.
- **Using the TBD (To Be Determined) Approach:** When adding a conference whose Call for Papers (CFP) has not yet been released, please add it using projected dates (e.g., based on the previous year) and include a `tba: true` flag (or your chosen indicator for TBD status) in the YAML entry. This allows us to tentatively track upcoming deadlines even before official announcements. Once the official CFP is released, please update the entry with the correct dates and details, and remove the `tba: true` flag.
- Please do not remove past conferences, as they are kept for reference.
**Adding Conference Types:**
- Edit the **`./_data/types.yml`** file.


**Data Format Example:**
```yaml
- title: BestConf
  year: 2022
  id: bestconf22  # title as lower case + last two digits of year
  full_name: Best Conference for Anything  # full conference name
  link: link-to-website.com
  deadline: 'YYYY-MM-DD HH:SS' # Use 24-hour format, inside quotes
  abstract_deadline: 'YYYY-MM-DD HH:SS' # Optional, inside quotes
  timezone: Asia/Seoul # Reference: https://momentjs.com/timezone/
  place: Incheon, South Korea
  date: September, 18-22, 2022 # Conference dates
  start: 'YYYY-MM-DD' # Conference start date, inside quotes
  end: 'YYYY-MM-DD' # Conference end date, inside quotes
  paperslink: link-to-full-paper-list.com # Optional
  pwclink: link-to-papers-with-code.com # Optional
  hindex: 100.0 # Optional, h5-index from Google Scholar
  sub: SP # Conference category/type from types.yml
  note: Important # Optional note
  tba: true # Optional: Use this flag if the CFP is not out yet (see Contributing section)
```
## Related Projects & Original Forks

This list includes other forks and related deadline projects, primarily from the ecosystem around the original `aideadlin.es`:

  - [geodeadlin.es][3] by @LukasMosser
  - [neuro-deadlines][4] by @tbryn
  - [ai-challenge-deadlines][5] by @dieg0as
  - [CV-oriented ai-deadlines (with an emphasis on medical images)][8] by @duducheng
  - [es-deadlines (Embedded Systems, Computer Architecture, and Cyber-physical Systems)][9] by @AlexVonB and @k0nze
  - [2019-2020 International Conferences in AI, CV, DM, NLP and Robotics][10] by @JackieTseng
  - [ccf-deadlines][11] by @ccfddl
  - [netdeadlines.com][12] by @albertgranalcoz
  - [ad-deadlines.com][13] by @daniel-bogdoll
  - [sec-deadlines.github.io/ (Security and Privacy)][14] by @clementfung
  - [pythondeadlin.es][15] by @jesperdramsch

## License

This project is licensed under the MIT License. See the [LICENSE](https://www.google.com/search?q=LICENSE) file for details.
This license is inherited from the original [abhshkdz/ai-deadlines](https://github.com/abhshkdz/ai-deadlines) project.

It uses icons from [IcoMoon Icons](https://icomoon.io/#icons-icomoon), licensed under [GPL](http://www.gnu.org/licenses/gpl.html) / [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/).

[3]: https://github.com/LukasMosser/geo-deadlines
[4]: https://github.com/tbryn/neuro-deadlines
[5]: https://github.com/dieg0as/ai-challenge-deadlines
[8]: https://m3dv.github.io/ai-deadlines/
[9]: https://ekut-es.github.io/es-deadlines/
[10]: https://jackietseng.github.io/conference_call_for_paper/conferences.html
[11]: https://ccfddl.github.io/
[12]: https://netdeadlines.com/
[13]: https://ad-deadlines.com/
[14]: https://sec-deadlines.github.io/
[15]: https://pythondeadlin.es/
