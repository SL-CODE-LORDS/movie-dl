<p align="center">
  <a href="" rel="noopener">
 <img width=150px height=50px src="https://sinhalasub.lk/wp-content/uploads/2020/11/2019.10.7.19h56m33sLAY0.png" alt="sinhalasub"></a>
</p>


<h2 align="center">SinhalaSub.LK Movie Downloader</h2>





## 📝 Table of Contents

- [About](#about)
- [Getting Started](#getting_started)
- [Usage](#usage)
- [Authors](#authors)

## 🧐 About <a name = "about"></a>

The unofficial Scrap <a href="https://sinhalasub.lk/" > [https://sinhalasub.lk/] </a>

## 🏁 Getting Started <a name = "getting_started"></a>

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Installing


```sh
yarn add @sl-code-lords/movie-dl
```

or

```sh
npm i @sl-code-lords/movie-dl
```

## 🎈 Usage <a name="usage"></a>

```ts
var { SinhalaSub }  = require('@sl-code-lords/movie-dl')

```
## Get Movies/Twshows List 


```ts
// By Search
var input = 'money heist' //movie or tvshow name
await SinhalaSub.get_list.by_search(input) 

// BY Recently added movies 
var page = 1 //page number
await SinhalaSub.get_list.by_recent_movies(page)

// Get Recently added tvshows list
var page = 1 //page number
await SinhalaSub.get_list.by_recent_tvshows(page)

// Get Movies/Tvshows List By Language
var lang = 'English' // Language ( ex : Sinhala , English , Tamil , Hindi , Kannada , France , Japanese , Telugu , Malayalam , Korean , Other )
var page = 1 //page number
await SinhalaSub.get_list.by_language[lang](page)

// Get Movies/Tvshows List By Genre
var genre = 'Action' // Genre ( ex : History , Thriller , Comedy ,  Horror , Adventure , Science_fiction , Mystery , Animation , Sport ,  Drama , Action , Crime , Romance , Fantasy , Family , War , Adult_only , Short )
var page = 1 //page number
await SinhalaSub.get_list.by_genre[genre](page)

// Get Movies/Tvshows List By Year
var year = '2023' // year
var page = 1 //page number
await SinhalaSub.get_list.by_year(year,page)

// Get Movies/Tvshows List By Actor
var url = 'https://sinhalasub.lk/cast/dhanush/' // cast link
var page = 1 //page number
await SinhalaSub.get_list.by_actor(url,page)

// Get Movies/Tvshows List By Director
var url = 'https://sinhalasub.lk/director/s-s-rajamouli/' // director url
var page = 1 //page number
await SinhalaSub.get_list.by_director(url,page)
```
```ts

//The results will look like this.

{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  results: [
    {
      title: 'Money Heist (2017 – 2021) Sinhala Subtitles | සිංහල උපසිරසි සමඟ',
      link: 'https://sinhalasub.lk/tvshows/money-heist-2017-sinhala-subtitles/',
      type: 'tvshows'
    },
    {
      title: 'Money Plane (2020) Sinhala Subtitles | සිංහල උපසිරසි සමඟ',
      link: 'https://sinhalasub.lk/movies/money-plane-2020-sinhala-subtitles/',
      type: 'movies'
    },
   2 more...
  ]
}
```
## Get Movie Details and Download Links
```ts
var url = 'https://sinhalasub.lk/movies/rrr-2022-sinhala-subtitles/' // movie url
await SinhalaSub.movie(url)
```
```ts
//result
{
  "status": true,
  "code_creator": {
    "name": "Thisal Sanujaya",
    "github": "@sanuwaofficial"
  },
  "result": {
    "title": "RRR (2022) Sinhala Subtitles | සිංහල උපසිරසි සමඟ",
    "subtitle_author": "రౌద్రం రణం రుధిరం",
    "categories": ["Action","Drama","History","Telugu","War"],
    "release_date": "Mar. 24, 2022",
    "country": "India",
    "duration": "187 Min.",
    "director": { "name": "S.S. Rajamouli","link": "https://sinhalasub.lk/director/s-s-rajamouli/"},
    "cast": [
      {"name": "N.T. Rama Rao Jr.","link": "https://sinhalasub.lk/cast/n-t-rama-rao-jr/"},
      {"name": "Ram Charan","link": "https://sinhalasub.lk/cast/ram-charan/"},
      8 more...
    ],
    "desc": "",
    "images": [
      "https://sinhalasub.lk/wp-content/uploads/2022/03/u0XUBNQWlOvrh0Gd97ARGpIkL0-200x300.jpg",
      "https://images.hindustantimes.com/img/2022/04/01/1600x900/RRR-Movie-Review_1648825470847_1648825479894.jpg",
      "https://image.tmdb.org/t/p/original/mQBz0kkJw9gWW1accn1UIPVnvtL.jpg",
     8 more...
    ],
    "dl_links": [
      {
        "quality": "FHD 1080p",
        "size": "4.55 GB",
        "link": "https://001.sinhalaking.tk/0:/Movie/Telugu/RRR%20(2022)/www.SinhalaSub.net%20-%20RRR%20(2022)%20Telugu%20HQ%20HDRip%201080p.mp4"
      },
      {
        "quality": "HD 720p",
        "size": "2.03 GB",
        "link": "https://001.sinhalaking.tk/0:/Movie/Telugu/RRR%20(2022)/www.SinhalaSub.net%20-%20RRR%20(2022)%20Telugu%20HQ%20HDRip%20720p.mp4"
      },
    8 more...
    ]
  }
}

```
## Get Tvshow Details and episode Links
```ts
var url = 'https://sinhalasub.lk/tvshows/money-heist-2017-sinhala-subtitles/' // tvshow url
await SinhalaSub.tvshow(url)
```
```ts
//result

{
  status: true,
  code_creator: { name: 'Thisal Sanujaya', github: '@sanuwaofficial' },
  result: {
    title: 'Money Heist (2017 – 2021) Sinhala Subtitles | සිංහල උපසිරසි සමඟ',
    categories: [ 'Crime', 'Drama', 'Spanish'],
    info: {
      Original_title: "La Casa de Papel",
      TMDb_Rating: " 8.3 16,046 votes ",
      First_air_date: "May. 02, 2017",
      Last_air_date: "Dec. 03, 2021",
      Seasons: "3",
      Episodes: "41",
      Average_Duration: "70 minutes "
    },
    cast: [
           { name: 'Álvaro Morte', link: 'https://sinhalasub.lk/cast/alvaro-morte/' },
           { name: 'Úrsula Corberó', link: 'https://sinhalasub.lk/cast/ursula-corbero/' },
           8 more...
          ],
    links: [ 
            [
             { episode: '1 - 1',
               link: 'https://sinhalasub.lk/episodes/money-heist-s1e1/'},
             {
              episode: '1 - 2',
              link: 'https://sinhalasub.lk/episodes/money-heist-s1e2/' },
             11 more...
           ], 
           [
             { episode: '2 - 1',
               link: 'https://sinhalasub.lk/episodes/money-heist-s2e1/'},
             { episode: '2 - 2',
               link: 'https://sinhalasub.lk/episodes/money-heist-s2e2/' },
             7 more...
           ],
            3 more... 
          ]
  }
}
```
## Get Episode Details and download Links
```ts
var url = 'https://sinhalasub.lk/episodes/money-heist-s2e2/' // episode url
await SinhalaSub.episode(url)
```
```ts
//result
{
  "status": true,
  "code_creator": {
    "name": "Thisal Sanujaya",
    "github": "@sanuwaofficial"
  },
  "result": {
    "title": "Money Heist (2017 – 2021) Sinhala Subtitles | සිංහල උපසිරසි සමඟ: 2x2",
    "desc": "The Professor recruits Martin to put his brother’s plan into action and target the Bank of Spain. First step? Create total chaos.",
    "release_date": "Jul. 19, 2019",
    "images": [
      "https://image.tmdb.org/t/p/original/wg7nd7r0Iptr2W8kW37OSed1C4q.jpg",
      "https://image.tmdb.org/t/p/original/cwFuj35BzUNWSNSoAyOscwpAT2n.jpg"
    ],
    "dl_links": [
      {
        "quality": "HD 720p",
        "size": "470 MB",
        "link": "https://001.sinhalaking.tk/0:/TV/Money%20Heist%20(TV%20Series%202017%E2%80%932021)/S02/www.SinhalaSub.net%20-%20La.Casa.de.Papel.S02E02%20WEBRip%20720p.mp4"
      },
      {
        "quality": "HD 720p",
        "size": "470 MB",
        "link": "https://002.sinhalaking.tk/0:/TV/Money%20Heist%20(TV%20Series%202017%E2%80%932021)/S02/www.SinhalaSub.net%20-%20La.Casa.de.Papel.S02E02%20WEBRip%20720p.mp4"
      },
      {
        "quality": "HD 720p",
        "size": "470 MB",
        "link": "https://003.sinhalaking.tk/0:/TV/Money%20Heist%20(TV%20Series%202017%E2%80%932021)/S02/www.SinhalaSub.net%20-%20La.Casa.de.Papel.S02E02%20WEBRip%20720p.mp4"
      }
    ]
  }
}
```

## ✍️ Authors <a name = "authors"></a>

- [@sanuwaofficial](https://github.com/sanuwaofficial) - scraped project author

See also the list of [contributors](https://github.com/SL-CODE-LORDS/movie-dl/contributors) who participated in this project.
